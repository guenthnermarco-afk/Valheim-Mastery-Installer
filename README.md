# Valheim Mastery — 0.18.5

Valheim Mastery adds **22 skills** for combat, exploration, production and animal husbandry. Each skill has milestones and a Mastery Cape at level 100; mastering all 22 unlocks the animated Apex Cape. Slayer contracts, 30 prayers, rune magic and optional equipment quality extend character progression. English and German are supported.

Inspired by Old School RuneScape progression, adapted to Valheim. This independent fan-made mod is not affiliated with or endorsed by Jagex.

## New in 0.18.5

- Tamed animals now show a compact star row below their health bar, independent of creature model size. One through four stars remain gold; five stars remain pink. Wild creatures retain their existing star placement.
- Hit numbers now display whole values: 59.8 is shown as 60. Actual HP changes and network damage values retain their original precision; healing and blocked-hit labels remain intact.
- Hit numbers are 15% smaller. Irregular hit splashes with subtle texture replace the smooth rectangular plates; their bounds fit the rendered numbers, including larger values and native font-size variations. Text and splash remain centred as the popup fades.
- Released leeches and their young stay fed for 600 seconds instead of the native dynamically added Tameable default of 30 seconds. Both leech variants are covered; preparing an existing animal preserves its last feeding time, tame state and ownership.

## Animal husbandry

**Beastmaster** connects taming, riding, slaughter and breeding. Species unlocks lead from boars and chickens to large mountain drakes at level 90. Normal offspring can improve up to four stars without dropping below the stronger parent's inherited natural tier. Mutations produce four- or five-star animals in 14 colour variants, including animated Crystal and Ember forms. Stars one through four stay gold; five stars appear pink. Eligible native enemy spawns can reach five stars; fixed-level actors remain unchanged.

Tamed animal maximum health and absolute native health regeneration scale with the known caretaker's Beastmaster level, up to twice their baseline at level 100. Breeding checks become up to twice as frequent; pregnancy duration, food, calmness and population limits still apply. Mutation chance reaches 5% at level 100. Crystal and Ember each average one in 220 total births at level 100; five-star mutations reach 10% of successful mutations. These are random chances, not guaranteed birth counts. Tranquilizer targeting and accepted-hit status are corrected for deer; existing animals and XP are preserved.

About 30% of wild adult mountain drakes are three times native size; only these large drakes are tameable. Non-damaging tranquilizer arrows require six body hits or four head hits; then feed the landed animal. Existing tamed animals stay tame, and the saved size does not change when taming. Craftable saddles support bears and drakes.

Mounted drakes start on the ground. Hold **Jump / Space** to take off or climb and **Crouch / Left Ctrl** to descend; remapped native actions are respected. Both together cancel the vertical request. The configured **Block** action (default right mouse button) requests a controlled landing. Held-key look assistance adjusts the 6 m/s vertical command to 4.5–7.5 m/s, with smoother acceleration and braking. Primary attack fires three frost projectiles, with a six-second cooldown and no additional attack stamina cost.

Base dragon stamina is 180; Beastmaster 100 raises it to 270 without a cape. Flight consumes 3 per second and requires following mode, a suitable launch surface, no overload and at least 60% reserve to start. The Beastmaster Cape adds 20% capacity and doubles ground recovery. Packbond halves personal riding cost for 120 seconds, with a 360-second cooldown. Flights stay within a 450 m radius of takeoff and a 24 m height envelope above ground or water. The rider's normal carry limit remains.

Other systems include travel to your own longship or drakkar, all 22 skill icons and the complete Mastery list, special energy below the minimap and **Shift + R** to arm or cancel weapon specials. Apex requires Beastmaster alongside the other 21 skills.

The community leaderboard includes Beastmaster and all 22 skills. Viewing does not require participation. Opting in publishes your chosen character name, category and 22 XP values. Scores are self-reported, with Standard and Test/multiplier categories kept separate. You can leave and delete the public profile; keep its recovery access code private. Older 21-skill submissions preserve an already recorded Beastmaster value.

## Controls

| Action | Default |
|---|---|
| Equipped cape power | C |
| Apex cape power selection | Shift + C |
| Arm/cancel supported weapon special | Shift + R |
| Call your following, unmounted animals | Shift + T; Beastmaster 70 |
| Ship sail styling at controls | Shift + Use |
| Rune spell / spellbook | F4 / F5 |
| Dragon climb / descend | Held Jump / Crouch |
| Dragon landing request | Block (default right mouse button) |
| Dragon frost salvo | Primary attack |

Menus and text input take priority. Lox and supported tamed adult animals have Follow/Stay commands. Recalling pets requires a safe arrival point and does not promise that every portal journey transports animals. Use the in-game books, milestones and tooltips for item-specific actions.

## Installation and updates

Requires **BepInExPack_Valheim 5.4.2350**. Supported Valheim versions: **1.0.15, 1.0.16 and 1.0.17**. The package contains **Core 0.18.5, WorldFeatures 1.1.0 and HuntingPhysics 1.0.1**; use matching components and gameplay settings on clients and server.

Stop the game and server before replacing files. Back up characters, worlds and the complete Mastery configuration and journals. Install through a compatible mod manager or copy the three supplied plugin components into `BepInEx/plugins`; remove duplicate older copies. Preserve existing configuration rather than replacing it with a new preset.

New profiles use XP ×1. Existing progress and settings are retained. Apex is checked against all 22 level-100 skills: an old 21-skill entitlement does not grant access before Beastmaster 100. Previously tamed animals are retained; mixed historical Farming XP is not blindly reassigned to the new skill.

The optional Comfort Pack adds UI, inventory and building conveniences. Optional item quality, enemy gear drops and weapon specials are off in fresh Core configurations; enable matching rules on each peer if desired. AzuCraftyBoxes is optional for shared-area chest access and reserves.

## Wiki and support

[Bilingual gameplay wiki: skills, controls, animal husbandry and complete reference tables](https://thunderstore.io/c/valheim/p/ValheimMastery/Valheim_Mastery/wiki/6084-start-bedienung-und-wiki-ubersicht/)

[Report an issue](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/issues/new/choose) with component versions, mod list and reproduction steps. Remove private information from excerpts. See `NOTICE.md` for asset and compatibility notices. **Known limitation:** following animals can remain behind during portal travel. The whistle is a separate recall action with its own safe-arrival checks.

## Deutsch

Valheim Mastery ergänzt **22 Skills** für Kampf, Reisen, Herstellung und Tierhaltung. Jeder Skill hat Meilensteine und ab Level 100 ein Mastery-Cape; alle 22 zusammen schalten das animierte Apex-Cape frei. Slayer-Aufträge, 30 Gebete, Runenmagie und optionale Gegenstandsqualität erweitern den Fortschritt.

Seit 0.18.4: Nixen werden ab Tiermeister 5 zaehmbar und nutzen die bestehenden Futter-, Zucht-, Mutations- und Pflegeregeln. Weitere zahme erwachsene Tiere erhalten Folgen/Warten. Eigene farbige Hitsplashes zeigen Schaden und bestätigte Betäubung ohne geänderte Schadenswerte.

**Tiermeister** verbindet Zähmen, Reiten, Schlachten und Zucht. Freischaltungen reichen vom Wildschwein und Huhn bis zum großen Bergdrachen auf 90. Normale Nachzucht kann sich bis zu vier Sternen verbessern und fällt nicht unter die geerbte natürliche Sternestufe des stärkeren Elternteils. Mutationen erzeugen vier- oder fünfsternige Tiere in 14 Farbvarianten, darunter animierte Kristall- und Glutformen. Sterne eins bis vier bleiben gold, fünf Sterne erscheinen pink. Geeignete native Gegnerspawns können fünf Sterne erreichen; festgelegte Gegnerstufen bleiben unverändert.

Maximale Lebenspunkte und absolute native Lebensregeneration gezähmter Tiere steigen mit dem Tiermeister-Level des bekannten Betreuers bis auf das Doppelte bei 100. Paarungsprüfungen erfolgen bis zu doppelt so häufig; Schwangerschaft, Nahrung, Ruhe und Populationsgrenzen gelten weiterhin. Die Mutationschance erreicht bei 100 fünf Prozent. Kristall und Glut kommen dann jeweils im Mittel bei einer von 220 Geburten vor; fünfsternige Mutationen erreichen zehn Prozent erfolgreicher Mutationen. Es sind Zufallswahrscheinlichkeiten, keine garantierten Geburtenzahlen. Hirsch-Zielprüfung und Anzeige akzeptierter Betäubungstreffer sind korrigiert; bestehende Tiere und XP bleiben erhalten.

Rund 30% der wilden erwachsenen Bergdrachen haben dreifache Vanilla-Größe; nur diese sind zähmbar. Schadensfreie Betäubungspfeile benötigen sechs Körper- oder vier Kopftreffer. Danach den gelandeten Drachen füttern. Vorhandene zahme Tiere bleiben zahm, die gespeicherte Größe ändert sich beim Zähmen nicht. Bären- und Drachensättel sind herstellbar.

Aufgesessene Drachen beginnen am Boden. **Springen / Leertaste halten** startet den Flug oder lässt steigen; **Ducken / linke Strg halten** lässt sinken. Geänderte native Tasten werden berücksichtigt, beide gleichzeitig neutralisieren die Höhe. Die konfigurierte **Blocken**-Aktion (Standard rechte Maustaste) fordert eine kontrollierte Landung an. Bei gehaltener Taste unterstützt der Blick die Höhenanforderung zwischen 4,5 und 7,5 m/s um einen Grundwert von 6 m/s. Primärangriff löst alle sechs Sekunden drei Frostgeschosse aus, ohne zusätzliche Angriffsausdauer.

180 Grundausdauer werden mit Tiermeister 100 ohne Cape zu 270. Flug verbraucht 3 pro Sekunde; Start benötigt Folgenstatus, einen geeigneten Untergrund, keine Überlast und mindestens 60% Reserve. Das Tiermeister-Cape ergänzt 20% Kapazität und verdoppelt die Bodenerholung. Rudelbund halbiert 120 Sekunden die eigenen Reitkosten, mit 360 Sekunden Abklingzeit. Der Flug bleibt auf 450 m Radius um den Start und 24 m Höhe über Boden/Wasser begrenzt. Die normale Traglast des Reiters bleibt maßgeblich.

Weitere Systeme sind Schiffreisen zum eigenen Langschiff oder Drakkar, alle 22 Skill-Symbole und die vollständige Meisterschaftsliste. Spezialenergie steht unter der Minikarte, **Umschalt + R** merkt Waffenspezialangriffe vor oder löst die Vormerkung. **C** aktiviert die Cape-Kraft, **Umschalt + C** wählt beim Apex eine Kraft. **Umschalt + T** ruft ab Tiermeister 70 eigene folgende, ungerittene Tiere. Sichere Ankunftsplätze und normale Zugriffsregeln gelten weiterhin.

Die Community-Rangliste umfasst Tiermeister und alle 22 Skills. Anschauen erfordert keine Teilnahme. Erst eine Anmeldung veröffentlicht deinen gewählten Charakternamen, Kategorie und 22 XP-Werte. Es sind selbst gemeldete Werte; Standard und Test/Multiplikator werden getrennt geführt. Du kannst die Teilnahme beenden und das öffentliche Profil löschen. Den Wiederherstellungs-Zugangscode privat aufbewahren. Ältere Einreichungen mit 21 Skills erhalten einen bereits gespeicherten Tiermeisterwert.

Benötigt **BepInExPack_Valheim 5.4.2350** und Valheim **1.0.15, 1.0.16 oder 1.0.17**. **Core 0.18.5, WorldFeatures 1.1.0 und HuntingPhysics 1.0.1** gemeinsam auf Clients und Server installieren. Vor dem Austausch Spiel/Server stoppen und Charaktere, Welten, komplette Mastery-Konfiguration und Journale sichern. Doppelte alte Plugins entfernen; eigene Einstellungen erhalten. Neue Profile starten mit XP ×1.

Apex verlangt alle 22 Skills auf 100; die frühere Berechtigung mit 21 Skills ersetzt Tiermeister nicht. Bestehende zahme Tiere und Fortschritte bleiben erhalten. Alte gemischte Landwirtschafts-XP werden nicht pauschal neu verteilt. Comfort Pack und AzuCraftyBoxes sind optional; Gegenstandsqualität, Ausrüstungsbeute und Waffenspezialangriffe sind in frischen Core-Einstellungen zunächst aus.

Deutsch/englische Anleitungen und Tabellen stehen im Wiki. **Bekannte Einschränkung:** Folgende Tiere können bei Portalreisen zurückbleiben. Der Pfiff ist eine separate Abruffunktion mit eigener Prüfung sicherer Ankunftsplätze. Fehler mit Versionen und nachvollziehbarem Ablauf melden, private Angaben aus Ausschnitten entfernen.

## Änderungen in 0.18.5

- Zahme Tiere zeigen eine kompakte Sternreihe unter dem Lebensbalken, unabhängig von der Größe des Tiermodells. Ein bis vier Sterne bleiben goldfarben, fünf Sterne pink. Die Sternposition wilder Tiere bleibt erhalten.
- Trefferzahlen erscheinen ohne Nachkommastellen: 59,8 wird als 60 angezeigt. Tatsächliche Lebenspunktänderungen und Netzwerk-Schadenswerte behalten ihre Genauigkeit; Heilungs- und Blockiertexte bleiben erhalten.
- Trefferzahlen sind 15% kleiner. Unregelmäßige Hitsplashes mit dezenter Struktur ersetzen die glatten rechteckigen Plaketten; ihre Größe passt sich an die tatsächlich dargestellten Zahlen an, auch bei größeren Werten und nativen Schriftgrößen. Zahl und Hitsplash bleiben beim Ausblenden zentriert.
- Freigelassene Blutegel und ihre Jungtiere bleiben 600 statt 30 Sekunden satt. Beide Blutegelarten sind erfasst; die Vorbereitung bestehender Tiere erhält den letzten Fütterungszeitpunkt, Zähmzustand und Besitzer.
