{% comment %}
This file is licensed under the MIT License (MIT) available on
http://opensource.org/licenses/MIT.
{% endcomment %}
{% assign filename="_data/devdocs/en/fabcoin-core/rpcs/rpcs/stop.md" %}

##### Stop
{% include helpers/subhead-links.md %}

{% assign summary_stop="safely shuts down the Fabcoin Core server." %}

{% autocrossref %}

The `stop` RPC {{summary_stop}}

*Parameters: none*

*Result---the server is safely shut down*

{% itemplate ntpd1 %}
- n: "`result`"
  t: "string"
  p: "Required<br>(exactly 1)"
  d: "The string \"Fabcoin server stopping\""

{% enditemplate %}

*Example from Fabcoin Core 0.10.0*

{% highlight bash %}
fabcoin-cli -testnet stop
{% endhighlight %}

Result:

{% highlight text %}
Fabcoin server stopping
{% endhighlight %}

*See also: none*

{% endautocrossref %}
