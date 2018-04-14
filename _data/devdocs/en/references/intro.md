{% comment %}
This file is licensed under the MIT License (MIT) available on
http://opensource.org/licenses/MIT.
{% endcomment %}
{% assign filename="_data/devdocs/en/references/intro.md" %}

{% autocrossref %}

The Developer Reference aims to provide technical details and API information
to help you start building Fabcoin-based applications, but it is [not a
specification][]. To make the best use of
this documentation, you may want to install the current version of Fabcoin
Core, either from [source][core git] or from a [pre-compiled executable][core executable].

Questions about Fabcoin development are best asked in one of the
[Fabcoin development communities][dev communities].
Errors or suggestions related to
documentation on Fabcoins.info can be [submitted as an issue][docs issue]
or posted to the [fabcoin-documentation mailing list][].

In the following documentation, some strings have been shortened or wrapped: "[...]"
indicates extra data was removed, and lines ending in a single backslash "\\"
are continued below. If you hover your mouse over a paragraph, cross-reference
links will be shown in blue.  If you hover over a cross-reference link, a brief
definition of the term will be displayed in a tooltip.

{% endautocrossref %}

#### Not A Specification
{:.no_toc}
{% include helpers/subhead-links.md %}

{% autocrossref %}

The Fabcoins.info Developer Documentation describes how Fabcoin works to
help educate new Fabcoin developers, but it is not a specification---and
it never will be.

Fabcoin security depends on consensus. Should your program diverge from
consensus, its security is weakened or destroyed. The cause of the
divergence doesn't matter: it could be a bug in your program, it could
be an [error in this documentation][errors in docs] which you
implemented as described, or it could be you do everything right but
other software on the network [behaves unexpectedly][v0.8 chain
fork]. The specific cause will not matter to the users of your software
whose wealth is lost.

The only correct specification of consensus behavior is the actual
behavior of programs on the network which maintain consensus. As that
behavior is subject to arbitrary inputs<!--noref--> in a large variety
of unique environments, it cannot ever be fully documented here or
anywhere else.

However, the Fabcoin Core developers are working on making their
consensus code portable so other implementations can use it. Fabcoin
Core 0.10.0 will provide `libfabcoinconsensus`, a first attempt at
exporting some consensus code. Future versions of Fabcoin Core will
likely provide consensus code that is more complete, more portable, and
more consistent in diverse environments.

In addition, we also warn you that this documentation has not been
extensively reviewed by Fabcoin experts and so likely contains numerous
errors. At the bottom of the menu on the left, you will find links that
allow you to report an issue or to edit the documentation on GitHub.
Please use those links if you find any errors or important missing
information.

{% endautocrossref %}
