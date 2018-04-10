{% comment %}
This file is licensed under the MIT License (MIT) available on
http://opensource.org/licenses/MIT.
{% endcomment %}
{% assign filename="_data/devdocs/en/fabcoin-core/rpcs/rpcs/move.md" %}

##### Move
{% include helpers/subhead-links.md %}

{% assign summary_move="moves a specified amount from one account in your wallet to another using an off-block-chain transaction." %}

{% autocrossref %}

*Requires wallet support.*

The `move` RPC {{summary_move}}

{{WARNING}} `move` will be removed in a later version of Fabcoin
Core.  Use the RPCs listed in the See Also subsection below instead.

{{WARNING}} it's allowed to move more funds than are in an account,
giving the sending account a negative balance and giving the receiving
account a balance that may exceed the number of fabcoins in the wallet
(or the number of fabcoins in existence).

*Parameter #1---from account*

{% itemplate ntpd1 %}
- n: "From Account"
  t: "string"
  p: "Required<br>(exactly 1)"
  d: "The name of the account to move the funds from"

{% enditemplate %}

*Parameter #2---to account*

{% itemplate ntpd1 %}
- n: "To Account"
  t: "string"
  p: "Required<br>(exactly 1)"
  d: "The name of the account to move the funds to"

{% enditemplate %}

*Parameter #3---amount to move*

{% itemplate ntpd1 %}
- n: "Amount"
  t: "number (fabcoins)"
  p: "Required<br>(exactly 1)"
  d: "The amount of fabcoins to move"

{% enditemplate %}

*Parameter #4---an unused parameter*

{% itemplate ntpd1 %}
- n: "*Unused*"
  t: "number (int)"
  p: "Optional<br>(0 or 1)"
  d: "This parameter is no longer used. If parameter #5 needs to be specified, this can be any integer"

{% enditemplate %}

*Parameter #5---a comment*

{% itemplate ntpd1 %}
- n: "Comment"
  t: "string"
  p: "Optional<br>(0 or 1)"
  d: "A comment to assign to this move payment"

{% enditemplate %}

*Result---`true` on success*

{% itemplate ntpd1 %}
- n: "`result`"
  t: "bool"
  p: "Required<br>(exactly 1)"
  d: "Set to `true` if the move was successful"

{% enditemplate %}

*Example from Fabcoin Core 0.10.0*

Move 0.1 fabcoins from "doc test" to "test1", giving the transaction the
comment "Example move":

{% highlight bash %}
fabcoin-cli -testnet move "doc test" "test1" 0.1 0 "Example move"
{% endhighlight %}

Result:

{% highlight json %}
true
{% endhighlight %}

*See also*

* [ListAccounts][rpc listaccounts]: {{summary_listAccounts}}
* [SendFrom][rpc sendfrom]: {{summary_sendFrom}}
* [SendToAddress][rpc sendtoaddress]: {{summary_sendToAddress}}

{% endautocrossref %}
