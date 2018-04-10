{% comment %}
This file is licensed under the MIT License (MIT) available on
http://opensource.org/licenses/MIT.
{% endcomment %}
{% assign filename="_data/devdocs/en/examples/testing.md" %}

## Testing Applications
{% include helpers/subhead-links.md %}

{% autocrossref %}

Fabcoin Core provides testing tools designed to let developers
test their applications with reduced risks and limitations.

{% endautocrossref %}

### Testnet
{% include helpers/subhead-links.md %}

{% autocrossref %}

When run with no arguments, all Fabcoin Core programs default to Fabcoin's main
network ([mainnet][/en/glossary/mainnet]{:#term-mainnet}{:.term}). However, for development,
it's safer and cheaper to use Fabcoin's test network (testnet)
where the satoshis spent have no real-world value. Testnet also relaxes some
restrictions (such as standard transaction checks) so you can test functions
which might currently be disabled by default on mainnet.

To use testnet, use the argument `-testnet`<!--noref--> with `fabcoin-cli`, `fabcoind` or `fabcoin-qt` or add
`testnet=1`<!--noref--> to your `fabcoin.conf` file as [described earlier][fabcoind initial setup].  To get
free satoshis for testing, use [Piotr Piasecki's testnet faucet][].
Testnet is a public resource provided for free by members of the
community, so please don't abuse it.

{% endautocrossref %}

### Regtest Mode
{% include helpers/subhead-links.md %}

{% autocrossref %}

For situations
where interaction with random peers and blocks is unnecessary or
unwanted, Fabcoin Core's regression test mode (regtest mode) lets you
instantly create a brand-new private block chain with the same basic
rules as testnet---but one major difference: you choose when to create
new blocks, so you have complete control over the environment.

Many developers consider regtest mode the preferred way to develop new
applications. The following example will let you create a regtest
environment after you first [configure fabcoind][fabcoind initial setup].

{% endautocrossref %}

{% highlight bash %}
> fabcoind -regtest -daemon
Fabcoin server starting
{% endhighlight %}

{% autocrossref %}

Start `fabcoind` in regtest mode to create a private block chain.

{% endautocrossref %}

~~~
## Fabcoin Core 0.10.1 and earlier
fabcoin-cli -regtest setgenerate true 101

## Fabcoin Core master (as of commit 48265f3)
fabcoin-cli -regtest generate 101
~~~

{% autocrossref %}

Generate 101 blocks using a special RPC
which is only available in regtest mode. This takes less than a second on
a generic PC. Because this is a new block chain using Fabcoin's default
rules, the first blocks pay a block reward of 50 fabcoins.  Unlike
mainnet, in regtest mode only the first 150 blocks pay a reward of 50 fabcoins.
However, a block must have 100 confirmations before that reward can be
spent, so we generate 101 blocks to get access to the coinbase
transaction from block #1.

{% endautocrossref %}

{% highlight bash %}
fabcoin-cli -regtest getbalance
50.00000000
{% endhighlight %}

{% autocrossref %}

Verify that we now have 50 fabcoins available to spend.

You can now use Fabcoin Core RPCs prefixed with `fabcoin-cli -regtest`<!--noref-->.

Regtest wallets and block chain state (chainstate) are saved in the `regtest`<!--noref-->
subdirectory of the Fabcoin Core configuration directory. You can safely
delete the `regtest`<!--noref--> subdirectory and restart Fabcoin Core to
start a new regtest. (See the [Developer Examples Introduction][devexamples] for default
configuration directory locations on various operating systems. Always back up
mainnet wallets before performing dangerous operations such as deleting.)

{% endautocrossref %}
