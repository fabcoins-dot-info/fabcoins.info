---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

layout: base-core
lang: en
columns: 1
id: fabcoin-core-requirements
title: Requirements And Warnings - Fabcoin Core
breadcrumbs:
  - fabcoin
  - bcc
  - bcc features
  - Requirements
---
# Fabcoin Core Requirements And Warnings
{:.not-displayed}

![Fabcoin Core requirements and warnings](/img/fabcoin-core/slider-warning.svg)

{% include fabcoin-core/download-fabcoin-core.html %}

Fabcoin Core gives you increased [security][bcc validation] and
[privacy][bcc privacy] at a cost. You need to [take
responsibility](#wallet-responsibility-checklist) for the security of
your fabcoins, meet higher [minimum system
requirements](#system-requirements), and beware of some [possible
problems](#possible-problems).

![Warning icon](/img/icons/icon_warning.svg)
**No matter what Fabcoin software you use,** you should never
buy more fabcoins than you can afford to lose. Fabcoin is still an
experimental system and fabcoins remain a risky investment.

## Wallet Responsibility Checklist

Fabcoin Core puts you in charge of your wallet, which means your
fabcoins are at risk unless you complete certain tasks:

{% comment %}
<!-- Note: the short pop-ups below are a temporary measure.  I (@harding) plan
to write a Fabcoin Core user guide for the site that will provide more
detailed instructions for at least some of these things. -->
{% endcomment %}

- <button class="popup js" data-container="backup_your_keys">Backup your keys</button>

- Make sure your <button class="popup js" data-container="secure_your_wallet">wallet is secure</button>

- Setup an <button class="popup js" data-container="offline_wallet">offline wallet</button>
  (cold storage) for significant amounts of fabcoins

- Watch for [security notifications](/en/alerts)

- Allow your heirs to <button class="popup js" data-container="fabcoin_inheritance">receive your fabcoins</button>
  if you die or become incapacitated

If you need help with any step, please ask for assistance in any of
Fabcoin's [friendly forums][bcc forums] or [live chatrooms][bcc live
help].

## System Requirements

{% assign DISK='<span class="fa fa-li fa-hdd-o fa-2x"></span> **Disk space**<br>' %}
{% assign DOWNLOAD='<span class="fa fa-li fa-download fa-2x"></span> **Download**<br>' %}
{% assign UPLOAD='<span class="fa fa-li fa-upload fa-2x"></span> **Upload**<br>' %}
{% assign MEMORY='<span class="fa fa-li fa-database fa-2x"></span> **Memory (RAM)**<br>' %}
{% assign SYSTEM='<span class="fa fa-li fa-desktop fa-2x"></span> **System**<br>' %}
{% assign OS='<span class="fa fa-li fa-windows fa-2x"></span> **Operating system**<br>' %}
{% assign FOOTNOTE='<b>*</b>' %}
{% capture INITIAL_DOWNLOAD %}<b>*</b> Plus a one-time {{site.text.chain_gb}} GB download the first time you start Fabcoin Core.{% endcapture %}

<div markdown="block" class="two-column-list" id="system-requirements-accordion">

### Bare Minimum (With Default Settings)

<div markdown="block">

{:.fa-ul}
- {{DISK}} {{site.text.fabcoin_datadir_gb}} GB

- {{DOWNLOAD}} 250 MB/day (8 GB/month){{FOOTNOTE}}

- {{UPLOAD}} 5 GB/day (150 GB/month)

- {{MEMORY}} 512 MB

- {{SYSTEM}} Desktop<br
  >Laptop<br
  >[Some ARM chipsets][wiki fabcoin core compatible devices arm] >1 GHz

- {{OS}} Windows 7/8.x<br
  >Mac OS X<br
  >Linux<br
  >Some BSDs

<br class="clear">

{{INITIAL_DOWNLOAD}}


</div>

### Bare Minimum (With Custom Settings)

<div markdown="block">

{:.fa-ul}
- {{DISK}} {{site.text.fabcoin_datadir_gb_pruned}} GB

- {{DOWNLOAD}} 150 MB/day (5 GB/month){{FOOTNOTE}}

- {{UPLOAD}} 10 MB/day (300 MB/month)

- {{MEMORY}} 256 MB

- {{SYSTEM}} Desktop<br
  >Laptop<br
  >[Most ARM chipsets][wiki fabcoin core compatible devices arm]

- {{OS}} Windows 7/8.x<br
  >Mac OS X<br
  >Linux<br
  >Some BSDs

<br class="clear">

{{INITIAL_DOWNLOAD}}

**Learn more:** [Fabcoin Core configuration options][bcc configuration]


</div>

### Minimum Recommended

<div markdown="block">

{:.fa-ul}
- {{DISK}} {{site.text.fabcoin_datadir_gb}} GB

- {{DOWNLOAD}} 500 MB/day (15 GB/month){{FOOTNOTE}}

- {{UPLOAD}} 5 GB/day (150 GB/month)

- {{MEMORY}} 1 GB

- {{SYSTEM}} Desktop<br
  >Laptop<br
  >[Some ARM chipsets][wiki fabcoin core compatible devices arm] >1 GHz

- {{OS}} Windows 7/8.x/10<br
  >Mac OS X<br
  >Linux

<br class="clear">

{{INITIAL_DOWNLOAD}}


</div>

</div>

## Possible Problems

{% include fabcoin-core/fabcoin-core-possible-problems.md %}

<div class="not-displayed">
  <div id="backup_your_keys" title="Backup Your Keys" markdown="block">
  By default, you need to backup Fabcoin Core after every 100
  transactions.  This includes both transactions you send as well as
  payments you request (whether or not you actually received the payment).

  For example, you need to backup after sending 33 payments and requesting
  67 payments (even though you only received 60 payments).

  Fabcoin Core can be configured to allow you to go more transactions
  between backups.  See the [`-keypool` setting][bcc configuration].
  </div>

  <div id="secure_your_wallet" title="Secure Your Wallet" markdown="block">
  Anyone who gets access to your wallet can steal your fabcoins.  The
  first line of defense against this is encrypting your wallet, an option
  from the File menu in the graphical interface.

  However, encrypting may not be enough if your computer becomes infected
  by malware.  Learn about <button class="popup js" data-container="offline_wallet">offline wallets</button>
  for security against this type of attack.

  In addition to securing your wallet, you also need to keep your backups
  secure.  Anyone who gets access to them can also steal your fabcoins.

  **Learn more:** [secure your wallet][]
  </div>

  <div id="offline_wallet" title="Offline Wallet" markdown="block">
  Computers that connect to the Internet are frequently hacked or infected
  with fabcoin-stealing malware.  Computers that never connect to the
  Internet are a much more secure location for your fabcoins.

  Fabcoin Core can be run on an always-offline computer, creating an
  offline wallet (also called a cold wallet).  The offline wallet will
  securely store the private keys, while a separate online Fabcoin Core
  wallet will send and receive transactions.

  **Learn more:** [Creating and signing offline transactions][offline transactions]
  </div>

  <div id="fabcoin_inheritance" title="Fabcoin Inheritance" markdown="block">
  Your Fabcoin wallet isn't like a bank account---it won't automatically
  go to your heirs if you die or become disabled.

  You have to plan ahead and make sure there is a way for your heirs
  to access your wallet backups when you're no longer available.

  **Learn more:** [Estate planning: how can I ensure my fabcoins are inheritable?][inherit fabcoins]

  </div>
</div>

<br class="clear big">
<div class="prevnext">
<span markdown="1">**Previous Feature**<br>[Privacy][bcc privacy]</span>
<span markdown="1">**Next feature**<br>[User interface][bcc user interface]</span>
</div>
<br class="clear">

{% include references.md %}
