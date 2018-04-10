---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

id: fabcoinwallet
title: "Fabcoin Wallet"
titleshort: "Fabcoin<br>Wallet"
compat: "mobile android blackberry"
level: 2
platform:
  - mobile:
    name: mobile
    os:
      - name: android
        text: "walletfabcoinwallet"
        link: "http://play.google.com/store/apps/details?id=de.schildbach.wallet"
        source: "http://github.com/fabcoin-wallet/fabcoin-wallet"
        screenshot: "fabcoinwalletandroid.png"
        check:
          control: "checkgoodcontrolfull"
          validation: "checkpassvalidationspvp2p"
          transparency: "checkpasstransparencyopensource"
          environment: "checkpassenvironmentmobile"
          privacy: "checkpassprivacybasic"
          fees: "checkgoodfeecontrolfull"
        privacycheck:
          privacyaddressreuse: "checkpassprivacyaddressrotation"
          privacydisclosure: "checkfailprivacydisclosurespv"
          privacynetwork: "checkfailprivacynetworknosupporttor"
      - name: blackberry
        text: "walletfabcoinwallet"
        link: "http://appworld.blackberry.com/webstore/content/23952882/"
        source: "http://github.com/fabcoin-wallet/fabcoin-wallet"
        screenshot: "fabcoinwalletandroid.png"
        check:
          control: "checkgoodcontrolfull"
          validation: "checkpassvalidationspvp2p"
          transparency: "checkpasstransparencyopensource"
          environment: "checkpassenvironmentmobile"
          privacy: "checkpassprivacybasic"
          fees: "checkgoodfeecontrolfull"
        privacycheck:
          privacyaddressreuse: "checkpassprivacyaddressrotation"
          privacydisclosure: "checkfailprivacydisclosurespv"
          privacynetwork: "checkfailprivacynetworknosupporttor"
---
