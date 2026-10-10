# Valheim Mastery — 0.18.13

## Änderungen

- Der kompakte P-Button sitzt wieder neben O unter der Inventarlast. Aktion und letztes Ergebnis stehen im Tooltip.
- Einlagern und Zutatenbereitstellung berücksichtigen alle normalen sichtbaren Inventarzeilen, auch durch EquipmentAndQuickSlots erweiterte Zeilen. Schnellleiste, Ausrüstung und reservierte Sonderplätze bleiben geschützt.
- Gebietslager protokollieren tatsächliche Aktionen, feste Ablehnungsgründe und aggregierte Mengen lokal. Keine Welt-, Spieler- oder Kistenkennungen werden in diese Meldungen aufgenommen.
- Freigelassene Blutegel und ihr Nachwuchs fressen rohes Wolfsfleisch. Der Futtertrog akzeptiert und verteilt es über die vorhandene Tierfütterung. Eine Portion sättigt weiterhin zehn Minuten; Zuchtwerte bleiben erhalten.

## Changes

- The compact P button is restored beside O beneath inventory weight. Its tooltip provides the action and most recent result.
- Deposit and ingredient staging include every ordinary visible inventory row, including EquipmentAndQuickSlots expansions. Hotbar, equipment and reserved special cells remain protected.
- Area storage logs actual actions, fixed rejection reasons and aggregate counts locally, without world, player or chest identifiers in these messages.
- Released leeches and their offspring eat raw wolf meat. Feeding troughs accept it and serve it through the existing animal-feeding path. Each serving still provides ten minutes of satiation; breeding values are retained.

Third-party modules and settings are retained. Only Core, its README and version information change in the embedded payload compared with V100.

## Retained changes from 0.18.10 / Übernommen aus 0.18.10

Text-or-icon signs, vanilla-sized tamed stars, preserved existing offspring ranks and the feeding fixes remain included. No new breeding-rate or loot/XP balance change is introduced by area storage.

Text-oder-Icon-Schilder, Vanilla-Sterne zahmer Tiere, erhaltener Nachkommenrang und die Fütterungsreparaturen bleiben enthalten. Gebietslager führen keine neue Vermehrungsrate oder Beute-/XP-Balanceänderung ein.

## Retained features from 0.18.7

- **Report a bug** opens a modal form from the inventory. Enter a title, description and optional reproduction steps. The form displays Mastery and game versions and opens a prefilled GitHub issue only when you click the button. You review and submit it with your GitHub account. No logs, saves, player/world identifiers or account data are attached. Copy report is available as a local fallback.
- Creature stars use vanilla size and position for wild and tamed animals: native one/two-star objects, matching gold sprites for three/four and pink for five.
- Eligible wild creatures have at least a 50% upgrade roll after reaching two stars; original entry, distance, fixed-level and boss restrictions remain. This is a conditional roll, not a 50% overall five-star spawn rate. At Beastmaster 100, normal offspring rank bonuses are +2 at 10%, +1 at 30%, otherwise unchanged, capped at four stars with inherited-tier protection. Five-star mutations reach 25% of successful mutations; the overall mutation cap remains 5%, and Crystal/Ember each remain one in 220 total births at level 100. Existing animals are not rerolled.
- Crafting gains eight optional local filters: All, Weapons, Armour, Tools, Ammo, Food, Potions and Other. Armour includes shields; Other includes materials. The native recipe list, scroll, selection, tooltips, upgrade tab, material payment and XP remain responsible. Native batch crafting and the existing level-75 queue (five jobs, ten with the Crafting Cape) are retained; no second queue or selectable specializations are introduced. Disable with `Interface/CraftingCategories`.
- Higher-star native loot scales more moderately. For zero through five stars, ordinary quantity factors are 1/2/4/6/8/10, while chance factors stop at 1/2/4/4/4/4. Trophy, quest/unique and unknown non-item quantities also stop at four. Native non-scaling, per-player and boss exceptions remain. Saved carcass loot and existing XP are not recalculated; these factors are not an overall expected-loot guarantee.
- Signs offer Text (no icon) or a centred known item icon. Equipment is excluded from new selections; saved equipment icons and stored text are preserved. Native access/permission checks and Interface/SignItemIcons remain.
- CSV escaping and row assembly move to the existing bounded background writer. Unity reads, sequence/timestamps and numeric formatting remain on the game thread. Format, order, rotation and counted overflow/error behavior are preserved. No general FPS or maximum-memory improvement is claimed.

## Animal husbandry

**Beastmaster** connects taming, riding, slaughter and breeding. Species unlocks lead from boars and chickens to large mountain drakes at level 90. Normal offspring can improve up to four stars without dropping below the stronger parent's inherited natural tier. Mutations produce four- or five-star animals in 14 colour variants, including animated Crystal and Ember forms. Stars one through four stay gold; five stars appear pink. Eligible native enemy spawns can reach five stars; fixed-level actors remain unchanged.

Tamed animal maximum health and absolute native health regeneration scale with the known caretaker's Beastmaster level, up to twice their baseline at level 100. Breeding checks become up to twice as frequent; pregnancy duration, food, calmness and population limits still apply. Mutation chance reaches 5% at level 100. Crystal and Ember each average one in 220 total births at level 100; five-star mutations reach 25% of successful mutations. These are random chances, not guaranteed birth counts. Tranquilizer targeting and accepted-hit status are corrected for deer; existing animals and XP are preserved.

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

Requires **BepInExPack_Valheim 5.4.2350**. Supported Valheim versions: **1.0.15, 1.0.16 and 1.0.17**. The package contains **Core 0.18.13, WorldFeatures 1.1.0 and HuntingPhysics 1.0.1**; use matching components and gameplay settings on clients and server.

Stop the game and server before replacing files. Back up characters, worlds and the complete Mastery configuration and journals. Install through a compatible mod manager or copy the three supplied plugin components into `BepInEx/plugins`; remove duplicate older copies. Preserve existing configuration rather than replacing it with a new preset.

New profiles use XP ×1. Existing progress and settings are retained. Apex is checked against all 22 level-100 skills: an old 21-skill entitlement does not grant access before Beastmaster 100. Previously tamed animals are retained; mixed historical Farming XP is not blindly reassigned to the new skill.

The optional Comfort Pack adds UI, inventory and building conveniences. Optional item quality, enemy gear drops and weapon specials are off in fresh Core configurations; enable matching rules on each peer if desired. Mastery area storage does not require AzuCraftyBoxes; its other optional integrations remain separate.

## Wiki and support

[Bilingual gameplay wiki: skills, controls, animal husbandry and complete reference tables](https://thunderstore.io/c/valheim/p/ValheimMastery/Valheim_Mastery/wiki/6084-start-bedienung-und-wiki-ubersicht/)

[Report an issue](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/issues/new/choose) with component versions, mod list and reproduction steps. Remove private information from excerpts. See `NOTICE.md` for asset and compatibility notices. **Known limitation:** following animals can remain behind during portal travel. The whistle is a separate recall action with its own safe-arrival checks.

## Deutsch

Valheim Mastery ergänzt **22 Skills** für Kampf, Reisen, Herstellung und Tierhaltung. Jeder Skill hat Meilensteine und ab Level 100 ein Mastery-Cape; alle 22 zusammen schalten das animierte Apex-Cape frei. Slayer-Aufträge, 30 Gebete, Runenmagie und optionale Gegenstandsqualität erweitern den Fortschritt.

Seit 0.18.4: Nixen werden ab Tiermeister 5 zaehmbar und nutzen die bestehenden Futter-, Zucht-, Mutations- und Pflegeregeln. Weitere zahme erwachsene Tiere erhalten Folgen/Warten. Eigene farbige Hitsplashes zeigen Schaden und bestätigte Betäubung ohne geänderte Schadenswerte.

**Tiermeister** verbindet Zähmen, Reiten, Schlachten und Zucht. Freischaltungen reichen vom Wildschwein und Huhn bis zum großen Bergdrachen auf 90. Normale Nachzucht kann sich bis zu vier Sternen verbessern und fällt nicht unter die geerbte natürliche Sternestufe des stärkeren Elternteils. Mutationen erzeugen vier- oder fünfsternige Tiere in 14 Farbvarianten, darunter animierte Kristall- und Glutformen. Sterne eins bis vier bleiben gold, fünf Sterne erscheinen pink. Geeignete native Gegnerspawns können fünf Sterne erreichen; festgelegte Gegnerstufen bleiben unverändert.

Maximale Lebenspunkte und absolute native Lebensregeneration gezähmter Tiere steigen mit dem Tiermeister-Level des bekannten Betreuers bis auf das Doppelte bei 100. Paarungsprüfungen erfolgen bis zu doppelt so häufig; Schwangerschaft, Nahrung, Ruhe und Populationsgrenzen gelten weiterhin. Die Mutationschance erreicht bei 100 fünf Prozent. Kristall und Glut kommen dann jeweils im Mittel bei einer von 220 Geburten vor; fünfsternige Mutationen erreichen 25 Prozent erfolgreicher Mutationen. Es sind Zufallswahrscheinlichkeiten, keine garantierten Geburtenzahlen. Hirsch-Zielprüfung und Anzeige akzeptierter Betäubungstreffer sind korrigiert; bestehende Tiere und XP bleiben erhalten.

Rund 30% der wilden erwachsenen Bergdrachen haben dreifache Vanilla-Größe; nur diese sind zähmbar. Schadensfreie Betäubungspfeile benötigen sechs Körper- oder vier Kopftreffer. Danach den gelandeten Drachen füttern. Vorhandene zahme Tiere bleiben zahm, die gespeicherte Größe ändert sich beim Zähmen nicht. Bären- und Drachensättel sind herstellbar.

Aufgesessene Drachen beginnen am Boden. **Springen / Leertaste halten** startet den Flug oder lässt steigen; **Ducken / linke Strg halten** lässt sinken. Geänderte native Tasten werden berücksichtigt, beide gleichzeitig neutralisieren die Höhe. Die konfigurierte **Blocken**-Aktion (Standard rechte Maustaste) fordert eine kontrollierte Landung an. Bei gehaltener Taste unterstützt der Blick die Höhenanforderung zwischen 4,5 und 7,5 m/s um einen Grundwert von 6 m/s. Primärangriff löst alle sechs Sekunden drei Frostgeschosse aus, ohne zusätzliche Angriffsausdauer.

180 Grundausdauer werden mit Tiermeister 100 ohne Cape zu 270. Flug verbraucht 3 pro Sekunde; Start benötigt Folgenstatus, einen geeigneten Untergrund, keine Überlast und mindestens 60% Reserve. Das Tiermeister-Cape ergänzt 20% Kapazität und verdoppelt die Bodenerholung. Rudelbund halbiert 120 Sekunden die eigenen Reitkosten, mit 360 Sekunden Abklingzeit. Der Flug bleibt auf 450 m Radius um den Start und 24 m Höhe über Boden/Wasser begrenzt. Die normale Traglast des Reiters bleibt maßgeblich.

Weitere Systeme sind Schiffreisen zum eigenen Langschiff oder Drakkar, alle 22 Skill-Symbole und die vollständige Meisterschaftsliste. Spezialenergie steht unter der Minikarte, **Umschalt + R** merkt Waffenspezialangriffe vor oder löst die Vormerkung. **C** aktiviert die Cape-Kraft, **Umschalt + C** wählt beim Apex eine Kraft. **Umschalt + T** ruft ab Tiermeister 70 eigene folgende, ungerittene Tiere. Sichere Ankunftsplätze und normale Zugriffsregeln gelten weiterhin.

Die Community-Rangliste umfasst Tiermeister und alle 22 Skills. Anschauen erfordert keine Teilnahme. Erst eine Anmeldung veröffentlicht deinen gewählten Charakternamen, Kategorie und 22 XP-Werte. Es sind selbst gemeldete Werte; Standard und Test/Multiplikator werden getrennt geführt. Du kannst die Teilnahme beenden und das öffentliche Profil löschen. Den Wiederherstellungs-Zugangscode privat aufbewahren. Ältere Einreichungen mit 21 Skills erhalten einen bereits gespeicherten Tiermeisterwert.

Benötigt **BepInExPack_Valheim 5.4.2350** und Valheim **1.0.15, 1.0.16 oder 1.0.17**. **Core 0.18.13, WorldFeatures 1.1.0 und HuntingPhysics 1.0.1** gemeinsam auf Clients und Server installieren. Vor dem Austausch Spiel/Server stoppen und Charaktere, Welten, komplette Mastery-Konfiguration und Journale sichern. Doppelte alte Plugins entfernen; eigene Einstellungen erhalten. Neue Profile starten mit XP ×1.

Apex verlangt alle 22 Skills auf 100; die frühere Berechtigung mit 21 Skills ersetzt Tiermeister nicht. Bestehende zahme Tiere und Fortschritte bleiben erhalten. Alte gemischte Landwirtschafts-XP werden nicht pauschal neu verteilt. Comfort Pack und AzuCraftyBoxes sind optional; Gegenstandsqualität, Ausrüstungsbeute und Waffenspezialangriffe sind in frischen Core-Einstellungen zunächst aus.

Deutsch/englische Anleitungen und Tabellen stehen im Wiki. **Bekannte Einschränkung:** Folgende Tiere können bei Portalreisen zurückbleiben. Der Pfiff ist eine separate Abruffunktion mit eigener Prüfung sicherer Ankunftsplätze. Fehler mit Versionen und nachvollziehbarem Ablauf melden, private Angaben aus Ausschnitten entfernen.

## Übernommene Funktionen aus 0.18.7

- **Report a bug** öffnet im Inventar ein modales Formular für Titel, Beschreibung und optionale Reproduktionsschritte. Mastery- und Spielversion werden sichtbar ergänzt. Erst der eigene Klick öffnet ein vorausgefülltes GitHub-Issue; Prüfung und Versand erfolgen über das eigene GitHub-Konto. Logs, Saves, Spieler-/Weltnamen und Kontodaten werden nicht angehängt. Bericht kopieren dient als lokaler Ausweichweg.
- Wilde und zahme Tiere verwenden Vanilla-Größe und -Position: native Ein-/Zwei-Sternobjekte, passende goldene Sprites für drei/vier und pink für fünf.
- Geeignete wilde Tiere erhalten nach Erreichen von zwei Sternen mindestens 50% pro weiterem Aufstufungswurf. Native Einstiegs-, Distanz-, Feststufen- und Bossregeln gelten weiter. Das bedeutet nicht 50% Fünfsterntiere insgesamt. Bei Tiermeister 100 erhalten normale Nachkommen +2 Rang mit 10%, +1 mit 30%, sonst keinen Bonus; maximal vier Sterne und Schutz der geerbten Stufe bleiben. Fünf Sterne erreichen 25% erfolgreicher Mutationen; die Gesamtmutationschance bleibt maximal 5%, Kristall und Glut jeweils eine von 220 Gesamtgeburten auf Level 100. Bestehende Tiere werden nicht neu ausgewürfelt.
- Acht lokal abschaltbare Herstellungsfilter: Alle, Waffen, Rüstung, Werkzeuge, Munition, Nahrung, Tränke, Sonstiges. Rüstung enthält Schilde, Sonstiges unter anderem Materialien. Native Rezeptliste, Scrollen, Auswahl, Tooltips, Aufwertungsreiter, Materialzahlung und XP bleiben zuständig. Native Mehrfachherstellung und vorhandene Warteschlange ab Level 75 bleiben erhalten: fünf Aufträge, zehn mit Handwerkscape. Keine zweite Queue und keine wählbaren Spezialisierungen. Schalter: `Interface/CraftingCategories`.
- Hochsternbeute steigt moderater: Bei null bis fünf Sternen gelten gewöhnliche Mengenfaktoren 1/2/4/6/8/10 und Chancefaktoren 1/2/4/4/4/4. Trophäen, Quest-/Einzelgegenstände und unbekannte Nicht-Item-Drops bleiben auch in der Menge bei maximal Faktor vier. Native Ausnahmen für unskalierte Drops, Spieleranzahl und Bosse bleiben. Gespeicherte Kadaverbeute und vorhandene XP werden nicht neu berechnet; die Faktoren sind keine pauschale Garantie der erwarteten Gesamtbeute.
- Schilder bieten Text (kein Symbol) oder ein mittiges bekanntes Itemicon. Ausrüstung ist aus neuen Auswahlen ausgeschlossen; gespeicherte Ausrüstungsicons und Text bleiben erhalten. Native Rechteprüfungen und Interface/SignItemIcons bleiben.
- CSV-Escaping und Zusammensetzen der Zeilen laufen im vorhandenen begrenzten Hintergrundschreiber. Unity-Abfragen, Zeitstempel, Reihenfolge und Zahlenformatierung bleiben im Spielthread. Format, Rotation und gezählte Überlast-/Fehlerverluste bleiben erhalten. Kein pauschaler FPS- oder maximaler Speichervorteil wird zugesichert.
