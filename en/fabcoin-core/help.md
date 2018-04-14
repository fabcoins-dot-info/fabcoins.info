---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

layout: base-core
lang: en
id: fabcoin-core-help
columns: 1
title: Get Help - Fabcoin Core
breadcrumbs:
  - fabcoin
  - bcc
  - Help

end_of_page: |
  <script src="/js/devsearch.js"></script>
---
# Getting Help For Fabcoin Core

There are many ways to get help for Fabcoin Core, including
[documentation](#documentation), [forums](#forums), and [live chatrooms](#live).

<span class="fa fa-exclamation-triangle"></span> *To report an issue,
please see the [bug reporting][bcc contribute issues] page.*

## Documentation

Fabcoin Core currently doesn't have any cohesive or complete
documentation---but we hope to improve that situation soon. For now, you
can use the following resources:

- Fabcoin Wiki pages: [running Fabcoin][bcc configuration], [data
  directory][bcc data directory], and other articles in the [Fabcoin
  Core documentation category][wiki fabcoin core documentation].

    <form id="searchform" action="http://fabcoins.info/wikiw/index.php">
      <input id="searchInput" class="glossary_term" type="search" placeholder="Search the Fabcoin Wiki" name="search"></input>
    </form>

- The [developer reference][RPCs] provides complete documentation of the
  RPCs that can be used with `fabcoin-cli` or in third-party programs.
  The [REST][rest] interface is also fully documented.  Both can be searched
  using the box below:

    <input id="glossary_term" class="glossary_term" placeholder="Search the RPCs and more">

- The [bandwidth sharing guide][] describes installing Fabcoin Core in
  detail as well as opening port 8665 to allow other Fabcoin programs to
  download blocks and transactions from you.

## Forums

Fabcoin has a wide range of [communities][communities], but the following places
are the best place to ask for help using Fabcoin Core:

- [Fabcoin StackExchange][] is a community dedicated entirely to
  answering questions about Fabcoin and related technology.  Many
  questions about Fabcoin Core can be found under the [Fabcoin-Qt
  tag](http://fabcoin.stackexchange.com/questions/tagged/fabcoin-qt)

- [FabcoinTalk Technical Support][forum tech support] is a
  sub-forum dedicated to providing help for Fabcoin Core and other
  Fabcoin programs.

- [/r/FabcoinBeginners][fabcoin beginners] is a Reddit community for
  users who have questions about anything Fabcoin-related, including
  Fabcoin Core.

## Live

Internet Relay Chat (IRC) is the most popular way to get live online
help with Fabcoin Core. When you join an IRC chatroom, you must read
the topic (which is usually automatically displayed) to learn the rules
for that chatroom.

- [#fabcoin][] is the best place to ask general questions about
  Fabcoin Core.

- [#fabcoin-mining][] hosts discussion about Fabcoin mining, including
  decentralized mining using Fabcoin Core as part of the system.

- For more channels, please see the [comprehensive listing][irc channels]
  on the Fabcoin Wiki.

{% include references.md %}
