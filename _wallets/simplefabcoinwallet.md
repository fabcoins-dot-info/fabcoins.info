---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

id: simplefabcoinwallet
title: "Simple Fabcoin Wallet"
titleshort: "Simple<br>Fabcoin"
compat: "mobile android"
level: 2
platform:
  - mobile:
    name: mobile
    os:
      - name: android
        text: "walletsimplefabcoinwallet"
        link: "http://play.google.com/store/apps/details?id=com.btcontract.wallet"
        source: "http://github.com/btcontract/wallet"
        screenshot: "simplefabcoinwalletandroid.png"
        check:
          control: "checkgoodcontrolfull"
          validation: "checkpassvalidationspvp2p"
          transparency: "checkpasstransparencyopensource"
          environment: "checkpassenvironmentmobile"
          privacy: "checkpassprivacybasic"
          fees: "checkpassfeecontroldynamic"
        privacycheck:
          privacyaddressreuse: "checkpassprivacyaddressrotation"
          privacydisclosure: "checkfailprivacydisclosurespv"
          privacynetwork: "checkfailprivacynetworknosupporttor"
---
