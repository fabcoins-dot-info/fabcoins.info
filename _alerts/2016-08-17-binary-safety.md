---
## This file is licensed under the MIT License (MIT) available on
## http://opensource.org/licenses/MIT.

title: "0.13.0 Binary Safety Warning"
shorturl: "binary-safety"
active: false
banner: ""
---

## Summary

Fabcoins.info has reason to suspect that the binaries for the upcoming Fabcoin Core release will likely be targeted by
state sponsored attackers. As a website, Fabcoins.info does not have the technical resources to guarantee
that we can defend ourselves from attackers of this calibre. We ask the Fabcoin community,
and in particular the Chinese Fabcoin community to be extra vigilant when downloading binaries from our website.

In such a situation, not being careful before you download binaries could cause you to lose all your coins. This malicious software
might also cause your computer to participate in attacks against the Fabcoin network. We believe Chinese services such as pools and exchanges
are most at risk here due to the origin of the attackers.

## Mitigation

The hashes of Fabcoin Core binaries are cryptographically signed with [this key](http://fabcoins.info/laanwj-releases.asc) belonging to Fabcoin Core maintainer Wladimir J. van der Laan. Additional signatures from other developers can be found in the [gitian signatures repository](http://github.com/fabcoin-core/gitian.sigs).

We strongly recommend that you download Wladimir's key from multiple sources in addition to Fabcoins.info for comparison purposes. For example, you can cross reference Fabcoins.info's copy with the [fabcoin-dev mailing list](http://lists.linuxfoundation.org/pipermail/fabcoin-dev/2015-June/009045.html) where Wladimir signed a message containing the key's fingerprint (01EA5486DE18A882D4C2684590C8019E36C2E964), but we encourage you to seek out other sources as well in order to make sure you are verifying your download with the correct key. Furthermore, we recommend verifying your download using signatures from multiple developers using the gitian signatures repository.

It is always best practice to securely verify multiple signatures and hashes before running any Fabcoin Core binaries. This is the safest and most secure way to ensure that the binaries you're running are the same ones created by the Core Developers.
