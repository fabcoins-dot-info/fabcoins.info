---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

id: arcbit
title: "ArcBit"
titleshort: "ArcBit"
compat: "mobile desktop android ios windows mac linux"
level: 3
platform:
  - desktop:
    name: desktop
    default: &DEFAULT
      text: "walletarcbit"
      link: "http://chrome.google.com/webstore/detail/arcbit-fabcoin-wallet/dkceiphcnbfahjbomhpdgjmphnpgogfk"
      source: "http://github.com/arcbit/arcbit-web"
      screenshot: "arcbitdesktop.png"
      check:
        control: "checkgoodcontrolfull"
        validation: "checkfailvalidationcentralized"
        transparency: "checkfailtransparencyremote"
        environment: "checkfailenvironmentdesktop"
        privacy: "checkpassprivacybasic"
        fees: "checkpassfeecontroloverride"
      privacycheck:
        privacyaddressreuse: "checkpassprivacyaddressrotation"
        privacydisclosure: "checkfailprivacydisclosurecentralized"
        privacynetwork: "checkpassprivacynetworksupporttorproxy"
    os:
      - name: windows
        <<: *DEFAULT
      - name: mac
        <<: *DEFAULT
      - name: linux
        <<: *DEFAULT
  - mobile:
    name: mobile
    os:
      - name: ios
        text: "walletarcbit"
        link: "http://itunes.apple.com/app/arcbit-fabcoin-wallet/id999487888"
        source: "http://github.com/arcbit/arcbit-ios"
        screenshot: "arcbitios.png"
        check:
          control: "checkgoodcontrolfull"
          validation: "checkfailvalidationcentralized"
          transparency: "checkpasstransparencyopensource"
          environment: "checkpassenvironmentmobile"
          privacy: "checkpassprivacybasic"
          fees: "checkpassfeecontroloverride"
        privacycheck:
          privacyaddressreuse: "checkpassprivacyaddressrotation"
          privacydisclosure: "checkfailprivacydisclosurecentralized"
          privacynetwork: "checkfailprivacynetworknosupporttor"
      - name: android
        text: "walletarcbit"
        link: "http://play.google.com/store/apps/details?id=com.arcbit.arcbit"
        source: "http://github.com/arcbit/arcbit-android"
        screenshot: "arcbitios.png"
        check:
          control: "checkgoodcontrolfull"
          validation: "checkfailvalidationcentralized"
          transparency: "checkpasstransparencyopensource"
          environment: "checkpassenvironmentmobile"
          privacy: "checkpassprivacybasic"
          fees: "checkpassfeecontroloverride"
        privacycheck:
          privacyaddressreuse: "checkpassprivacyaddressrotation"
          privacydisclosure: "checkfailprivacydisclosurecentralized"
          privacynetwork: "checkfailprivacynetworknosupporttor"
---
