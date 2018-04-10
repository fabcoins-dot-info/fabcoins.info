{% comment %}
This file is licensed under the MIT License (MIT) available on
http://opensource.org/licenses/MIT.
{% endcomment %}
{% assign filename="_data/devdocs/en/fabcoin-core/rpcs/rpcs/getbalance.md" %}

##### GetBalance
{% include helpers/subhead-links.md %}

{% assign summary_getBalance="gets the balance in decimal fabcoins across all accounts or for a particular account." %}

{% autocrossref %}

*Requires wallet support.*

The `getbalance` RPC {{summary_getBalance}}

*Parameter #1---an account name*

{% itemplate ntpd1 %}
- n: "Account"
  t: "string"
  p: "Optional<br>(0 or 1)"
  d: "*Deprecated: will be removed in a later version of Fabcoin Core*<br><br>The name of an account to get the balance for.  An empty string (\"\") is the default account.  The string `*` will get the balance for all accounts (this is the default behavior)"

{% enditemplate %}

*Parameter #2---the minimum number of confirmations*

{{INCLUDE_CONFIRMATIONS_PARAMETER}}

*Parameter #3---whether to include watch-only addresses*

{{INCLUDE_INCLUDE_WATCH_ONLY_PARAMETER}}

*Result---the balance in fabcoins*

{% itemplate ntpd1 %}
- n: "`result`"
  t: "number (fabcoins)"
  p: "Required<br>(exactly 1)"
  d: "The balance of the account (or all accounts) in fabcoins"

{% enditemplate %}

*Examples from Fabcoin Core 0.10.0*

Get the balance for the "test1" account, including transactions with
at least one confirmation and those spent to watch-only addresses in
that account.

{% highlight bash %}
fabcoin-cli -testnet getbalance "test1" 1 true
{% endhighlight %}

Result:

{% highlight json %}
1.99900000
{% endhighlight %}

*See also*

* [ListAccounts][rpc listaccounts]: {{summary_listAccounts}}
* [GetReceivedByAccount][rpc getreceivedbyaccount]: {{summary_getReceivedByAccount}}
* [GetReceivedByAddress][rpc getreceivedbyaddress]: {{summary_getReceivedByAddress}}

{% endautocrossref %}
