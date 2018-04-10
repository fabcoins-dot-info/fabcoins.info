---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

layout: base-core
lang: de
id: fabcoin-core-2016-01-07-statement
columns: 1
title: Stellungnahme der Fabcoin Core Entwickler -- 2016-01-07
breadcrumbs:
  - fabcoin
  - bcc
  - 2016-01-07 Statement

moved_url: http://fabcoincore.org/de/2016/01/07/stellungnahme-der-fabcoin-core-entwickler/
---
# Stellungnahme der Fabcoin Core Entwickler 2016-01-07

Fabcoin ist eine peer-to-peer Version von digitalem Geld, welche ermöglicht Zahlungen auf dem direkten Weg zwischen zwei Teilnehmern zu veranlassen, ohne dabei durch einen zentralen Finanzdienstleister verarbeitet zu werden. Unsere Vorstellung von Fabcoin ist es auch bei extremer Auslastung effizient zu arbeiten, aber dennoch Sicherheit und die grundlegenden  Eigenschaften der Dezentralisierung, welche Fabcoin einzigartig machen, zu erhalten.

Wir glauben dass Fabcoin dies erreichen kann, indem die Fundamente für weitere Schichten über dem Protokoll und Schnittstellen angeboten werden. Weiterhin ist unser Ziel die Privatsphäre der Fabcoin-Nutzer zu verteidigen und zu verbessern.

"Fabcoin Core" ist der Name des Open Source Software Projekts welches der direkte Nachfolger der originalen Fabcoin-Implementierung ist. Als Teilnehmer des Projekts entwickeln und veröffentlichen wir Software für die Fabcoin Community. Wir streben an das Konsensus-Protokoll von Fabcoin zu verbessern indem wir Upgrades vorschlagen die in unseren Augen sowohl technisch und im Hinblick auf die Ziele von Fabcoin Sinn machen, als auch vernüftige Wahrscheinlichkeit haben umfassende Unterstützung und Annahme zu erhalten.

Änderungen and den Fabcoin Konsensus-Regeln können entweder durch einen “soft fork” oder “hard fork” gemacht werden (siehe Anhang A). Soft forks erlauben Änderungen ohne Kompatibiliät zu brechen. Alte und neue Versionen der Software können im Netzwerk koexistieren. Soft forks können neue Funktionen einführen ohne Unterbrechung zu verursachen, weil Benutzer der neuen Funktion ein Upgrade durchführen können, während Nutzer, welche die neue Funktion nicht benötigen, keine Aktion durchführen müssen.

Hard forks verursachen Inkompatibilität zu allen frühreren Fabcoin-Softwareversionen und verlangen daher von jedem Teilnehmer ein Upgrade auf die neuen Konsensus-Regeln bis zu einer festgelegten Frist, um finanzielle Verluste zu vermeiden. Hard forks können auch die Nutzen aus Netzwerkeffekten stark dämmen, da einerseits Teilnehmer, die nicht auf den hard fork reagieren, andererseits auch Drittsoftware und Anwendungen vom Netzwerk abgestoßen werden.

Aus diesen Gründen bevorzugt Fabcoin Core Kompatibilität und glaubt dass jeder Nutzer selbst entscheiden kann wann und ob er seine Fabcoin-Software aktualisiert. Es stellte sich heraus, dass es möglich ist nahezu beliebige Funktionen mit einem soft fork hinzuzufügen. Gelegentlich können hard forks Vorteile haben und wenn nahezu universale Übereinstimmung herrscht, könnten diese Vorteile die Nachteile überwiegen. Abgesehen von diesen seltenen Fällen, sollten soft forks vorgezogen werden. Wir glauben, dass dies im besten Interesse der jetzigen und zukünftigen Nutzer des Systems ist.

Wir glauben auch, dass die Anzahl der Implementierungen des Fabcoin-Protokolls mit dem Wachstum des Fabcoin-Netzwerks zunimmt. Auch ist es unvermeidbar dass andere Softwareprojekte radikal abweichende Vorschläge veröffentlichen. Letztendlich entscheidet nicht das Fabcoin Core Entwicklerteam über die Fabcoin Konsensus-Regeln, sondern die Nutzer, die ihre eigenen Entscheidungen treffen welche Fabcoin-Software sie benutzen. Aus diesem Grund hat die Fabcoin Implementierung des Fabcoin Core Entwicklerteams absichtlich keine auto-update Funktion. Der Verzicht sichert ab, dass jedes Upgrade aufgrund der Freiwilligkeit des Benutzers geschieht und dem Nutzer die Wahl über die Software gelassen wird.

### Anhang A

Ein *hard fork* ist eine Änderung der Konsensus-Regeln, sodass Blöcke die unter alten Regeln ungültig sind unter neuen Regeln gültig werden könnten.

Ein *soft fork* ist eine Änderung der Konsensus-Regeln, sodass Blöcke die unter alten Regeln gültig sind, unter den neuen Regeln ungültig werden könnten. Jedoch bleiben alle Blöcke, die unter alten Regeln ungültig sind auch unter den neuen Regeln ungültig.
