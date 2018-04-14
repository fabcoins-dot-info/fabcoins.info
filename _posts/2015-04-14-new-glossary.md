---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

type: posts
layout: post
category: blog

title: "Dev Docs: New Glossary And Search Feature"
permalink: /en/posts/developer-docs-glossary-and-search.html
date: 2015-04-14
author: >
  David A. Harding (<a href="mailto:dave@dtrt.org">email</a>, <a
  href="http://github.com/harding">GitHub</a>,
  <a href="http://www.reddit.com/user/harda/">Reddit</a>)
---

*Thanks to [several volunteers][] and the financial sponsorship of [The
Fab Foundation][], we've added two major new features to the
[Fabcoins.info Developer Documentation][].*

A new [glossary section][] has been added to the Fabcoins.info Developer
Documentation, and with it comes a fully-Javascript search engine that
helps you look up glossary entries, Fabcoin Core RPCs, Fabcoin BIPs,
Script-language opcodes, and Fabcoin P2P protocol messages.

## Developer glossary main page

![Developer glossary main page](/img/blog/free/devglossary-main-page.png)

The glossary main page provides a search box and a sorted list of terms.
It uses a floating list so that it looks good on both mobiles and
desktop/laptop screens.

A link is provided at the bottom of the page to allow readers to
recommend new glossary terms. (It works like the Submit New Event link
on the [Events page][].)

### Glossary entries

![Glossary entries](/img/blog/free/devglossary-entries.png)

Each glossary entry has its own page providing a short definition
(limited to 255 characters), one or more synonyms, zero or more "not to
be confused with" terms, and zero or more links to resources on and off
Fabcoins.info. Separate pages were used to allow search engines to link
directly to the most relevant entry, rather than forcing users to scroll
through a giant page of definitions.

The glossary currently has:

* 89 glossary entry pages
* 51 additional synonyms
* 222 links (all internal to Fabcoins.info or to Fabcoin Wiki, FabcoinTalk, or Fabcoin StackExchange)

Each page includes links to edit it, view its history, or report an
issue about it.

### Dev search box

![Glossary search box](/img/blog/free/devglossary-search-box.png)

A Javascript-powered search box is added to the following pages: [Dev
Guide][], [Dev Reference][], [Dev Examples][], [Dev Glossary][], and individual
glossary entry pages.

The box allows finding the following by keyword, listed in the order
they appear in the search:

* Glossary entries (Fabcoins.info)
* RPCs  (Fabcoins.info)
* Opcodes (Fabcoin Wiki)
* BIPs (just notable and non-withdrawn BIPs; GitHub.com BIPs repo)
* Fabcoin P2P protocol messages (Fabcoins.info)

The search uses [JQuery][] and [JQuery UI][], both MIT-licensed. Both are
loaded from the Fabcoins.info server so there's no stats leakage when
people load them.

[dev guide]: /en/developer-guide
[dev reference]: /en/developer-reference
[dev examples]: /en/developer-examples
[dev glossary]: /en/developer-glossary
[jquery]: http://jquery.com/
[jquery ui]: http://jqueryui.com/
[several volunteers]: http://github.com/fabcoins-dot-info/fabcoins.info/pull/793
[Fabcoins.info developer documentation]: /en/developer-documentation
[the fabcoin foundation]: http://fabcoin.co/
[glossary section]: /en/developer-glossary
[events page]: /en/events
