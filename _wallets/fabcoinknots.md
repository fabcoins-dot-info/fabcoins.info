---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

id: fabcoinknots
title: "Fabcoin Knots"
titleshort: "Fabcoin<br>Knots"
compat: "desktop windows mac linux"
level: 1
platform:
  - desktop:
    name: desktop
    default: &DEFAULT
      text: "walletfabcoinknots"
      link: "http://fabcoinknots.org/"
      source: "http://github.com/fabcoinknots/fabcoin/"
      screenshot: "fabcoinknots.png"
      check:
        control: "checkgoodcontrolfull"
        validation: "checkgoodvalidationfullnode"
        transparency: "checkgoodtransparencydeterministic"
        environment: "checkfailenvironmentdesktop"
        privacy: "checkgoodprivacyimproved"
        fees: "checkgoodfeecontrolfull"
      privacycheck:
        privacyaddressreuse: "checkpassprivacyaddressrotation"
        privacydisclosure: "checkpassprivacydisclosurefullnode"
        privacynetwork: "checkpassprivacynetworksupporttorproxy"
    os:
      - name: windows
        <<: *DEFAULT
      - name: mac
        <<: *DEFAULT
      - name: linux
        <<: *DEFAULT
---
