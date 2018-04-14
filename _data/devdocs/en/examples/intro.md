{% comment %}
This file is licensed under the MIT License (MIT) available on
http://opensource.org/licenses/MIT.
{% endcomment %}
{% assign filename="_data/devdocs/en/examples/intro.md" %}

{% autocrossref %}

The following guide aims to provide examples to help you start
building Fabcoin-based applications. To make the best use of this document,
you may want to install the current version of Fabcoin Core, either from
[source][core git] or from a [pre-compiled executable][core executable].

Once installed, you'll have access to three programs: `fabcoind`,
`fabcoin-qt`, and `fabcoin-cli`.

* `fabcoin-qt` provides a combination full Fabcoin peer and wallet
  frontend. From the Help menu, you can access a console where you can
  enter the RPC commands used throughout this document.

* `fabcoind` is more useful for programming: it provides a full peer
  which you can interact with through RPCs to port 8667 (or 18667
  for testnet).

* `fabcoin-cli` allows you to send RPC commands to `fabcoind` from the
  command line.  For example, `fabcoin-cli help`

All three programs get settings from `fabcoin.conf` in the `Fabcoin`
application directory:

* Windows: `%APPDATA%\Fabcoin\`

* OSX: `$HOME/Library/Application Support/Fabcoin/`

* Linux: `$HOME/.fabcoin/`

To use `fabcoind` and `fabcoin-cli`, you will need to add a RPC password
to your `fabcoin.conf` file. Both programs will read from the same file
if both run on the same system as the same user, so any long random
password will work:

~~~
rpcpassword=change_this_to_a_long_random_password
~~~~

You should also make the `fabcoin.conf` file only readable to its
owner.  On Linux, Mac OSX, and other Unix-like systems, this can be
accomplished by running the following command in the Fabcoin application
directory:

~~~
chmod 0600 fabcoin.conf
~~~

For development, it's safer and cheaper to use Fabcoin's test network (testnet)
or regression test mode (regtest) described below.

Questions about Fabcoin use are best sent to the [FabcoinTalk forum][forum
tech support] and [IRC channels][]. Errors or suggestions related to
documentation on Fabcoins.info can be [submitted as an issue][docs issue]
or posted to the [fabcoin-documentation mailing list][].

In the following documentation, some strings have been shortened or wrapped: "[...]"
indicates extra data was removed, and lines ending in a single backslash "\\"
are continued below. If you hover your mouse over a paragraph, cross-reference
links will be shown in blue.  If you hover over a cross-reference link, a brief
definition of the term will be displayed in a tooltip.

{% endautocrossref %}
