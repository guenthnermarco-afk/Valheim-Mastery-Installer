# Valheim Mastery 0.18.23

22 Mastery skills with progression, capes, crafting, runic magic and Beastmaster animals. Supported Valheim versions: see the installed version check; this release is built against Valheim 1.0.17.

Release: 15 October 2026 / 15.10.2026. Installer V111.

See [release notes / Versionshinweise](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/releases/tag/v0.18.23) for early magic, native interface styling and marked-junk deletion compatibility. Before upgrading, back up saves and Mastery journals. 0.18.20 and earlier cannot read the new hit-XP journal. Downgrade requires a coherent full pre-update backup of characters, worlds and combat journals, not only an older DLL.

Vor dem Update Charaktere, Welten und Mastery-Journale sichern. 0.18.20 und älter lesen das neue Treffer-XP-Journal nicht; ein Downgrade benötigt eine zusammengehörige vollständige Vorupdate-Sicherung, nicht nur eine ältere DLL.

## Storage and crafting / Lager und Herstellung

When installed, AzuCraftyBoxes and QuickStackPlus handle crafting resources and storage by default. The full Windows installer also includes its routing extension; the Core and Comfort packages do not supply that custom routing extension. Mastery's native area transactions are disabled. The original QuickStackPlus P button remains in use. External plugins keep their own configured ranges and filters; this mode does not claim unlimited access to every chest in a building area.

Installierte AzuCraftyBoxes und QuickStackPlus übernehmen standardmäßig Ressourcen und Lagerung. Der vollständige Windows-Installer enthält zusätzlich seine Routing-Erweiterung; die Core- und Comfort-Pakete liefern diese eigene Routing-Erweiterung nicht mit. Masterys eigene Gebietstransaktionen sind ausgeschaltet. Der ursprüngliche QuickStackPlus-P-Button bleibt zuständig. Reichweite und Filter richten sich wieder nach den externen Mods.

`Storage / EnableNativeAreaStorage = false` is the default. Changes require a restart. Without the optional external plugins, native Valheim crafting and storage remain available.


## This update / Dieses Update

Added Pebble Bough at Magic 6 / Crafting 1, a Construction-1 Rune Forge and an in-game early-magic guide using actual recipe data. Grove Spark, Pebble Bough and Thorn Watch use new original models and icons. Mastery windows share native Valheim panels and readable fonts. A targeted fix restores explicit marked-junk deletion for the affected QuickStackPlus 1.1.2 binary. Existing progress and personal settings are retained.

Neu sind Kieselzweig ab Magie 6 / Handwerk 1, die Runenschmiede ab Baukunst 1 und eine Magie-Einstiegsanleitung aus tatsächlichen Rezeptdaten. Hainfunke, Kieselzweig und Dornwacht besitzen neue eigene Modelle und Icons. Masteryfenster verwenden native Holzpanels und passende Schriften. Eine gezielte Korrektur repariert den ausdrücklich ausgelösten Müll-Löschaufruf der betroffenen QuickStackPlus-1.1.2-Datei. Fortschritt und persönliche Einstellungen bleiben erhalten.

## Rune supply retained from 0.18.22 / Runenversorgung aus 0.18.22

Eligible natural enemy deaths give one guaranteed biome packet of 6/9/12 finished runes, plus a 60% chance for a supply packet of 3/6. Each packet adds 3 per star, up to five stars. Earlier reagents remain available later, while advanced types retain biome restrictions. More explicit natural species are supported. Blank-rune chance and per-drop quantities, recipes, spell costs and XP remain unchanged. See [release notes / Versionshinweise](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/releases/tag/v0.18.22) for all eight biome pools.

Geeignete natürliche Gegner geben ein garantiertes Biom-Paket mit 6/9/12 fertigen Runen und mit 60% Chance zusätzlich 3/6 Versorgungsrunen. Je Paket kommen 3 pro Stern hinzu, bis fünf Sterne. Frühe Reagenzien bleiben später verfügbar, fortgeschrittene Arten behalten ihre Biomgrenzen. Zusätzliche natürliche Spezies sind ausdrücklich aufgenommen. Rohlingchance und Mengen je Rohlingdrop, Rezepte, Zauberkosten und XP bleiben erhalten.

**Downgrade:** The hit-XP journal rule introduced in 0.18.21 remains. 0.18.20 and earlier cannot read it; restore a coherent full pre-update backup of characters, worlds and journals rather than mixing journal generations or replacing only the DLL.

**Downgrade:** Die Trefferjournal-Regel aus 0.18.21 gilt weiter. 0.18.20 und älter lesen dieses Journal nicht; vollständige zusammengehörige Vorupdate-Sicherung von Charakteren, Welten und Journalen verwenden, keine gemischten Generationen oder reine DLL-Rücksetzung.

## Retained features from 0.18.7

- **Report a bug** opens a modal form from the inventory. Enter a title, description and optional reproduction steps. The form displays Mastery and game versions and opens a prefilled GitHub issue only when you click the button. You review and submit it with your GitHub account. No logs, saves, player/world identifiers or account data are attached. Copy report is available as a local fallback.
- Creature stars use vanilla size and position for wild and tamed animals: native one/two-star objects, matching gold sprites for three/four and pink for five.
- Eligible wild creatures have at least a 50% upgrade roll after reaching two stars; original entry, distance, fixed-level and boss restrictions remain. This is a conditional roll, not a 50% overall five-star spawn rate. At Beastmaster 100, normal offspring rank bonuses are +2 at 10%, +1 at 30%, otherwise unchanged, capped at four stars with inherited-tier protection. Five-star mutations reach 25% of successful mutations; the overall mutation cap remains 5%. Existing animals are not rerolled.
- Crafting gains eight optional local filters: All, Weapons, Armour, Tools, Ammo, Food, Potions and Other. Armour includes shields; Other includes materials. The native recipe list, scroll, selection, tooltips, upgrade tab, material payment and XP remain responsible. Native batch crafting and the existing level-75 queue (five jobs, ten with the Crafting Cape) are retained; no second queue or selectable specializations are introduced. Disable with `Interface/CraftingCategories`.
- Higher-star native loot scales more moderately. For zero through five stars, ordinary quantity factors are 1/2/4/6/8/10, while chance factors stop at 1/2/4/4/4/4. Trophy, quest/unique and unknown non-item quantities also stop at four. Native non-scaling, per-player and boss exceptions remain. Saved carcass loot and existing XP are not recalculated; these factors are not an overall expected-loot guarantee.
- Signs offer Text (no icon) or a centred known item icon. Equipment is excluded from new selections; saved equipment icons and stored text are preserved. Native access/permission checks and Interface/SignItemIcons remain.
- CSV escaping and row assembly move to the existing bounded background writer. Unity reads, sequence/timestamps and numeric formatting remain on the game thread. Format, order, rotation and counted overflow/error behavior are preserved. No general FPS or maximum-memory improvement is claimed.

## Animal husbandry

**Beastmaster** connects taming, riding, slaughter and breeding. Species unlocks lead from boars and chickens to large mountain drakes at level 90. Normal offspring can improve up to four stars without dropping below the stronger parent's inherited natural tier. Mutations produce four- or five-star animals in multiple colour variants. Stars one through four stay gold; five stars appear pink. Eligible native enemy spawns can reach five stars; fixed-level actors remain unchanged.

Tamed animal maximum health and absolute native health regeneration scale with the known caretaker's Beastmaster level, up to twice their baseline at level 100. Breeding checks become up to twice as frequent; pregnancy duration, food, calmness and population limits still apply. Mutation chance reaches 5% at level 100. These are random chances, not guaranteed birth counts. Tranquilizer targeting and accepted-hit status are corrected for deer; existing animals and XP are preserved.

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

Requires **BepInExPack_Valheim 5.4.2350**. Supported Valheim versions: **1.0.15, 1.0.16 and 1.0.17**. The package contains **Core 0.18.23, WorldFeatures 1.1.0 and HuntingPhysics 1.0.1**; use matching components and gameplay settings on clients and server.

Stop the game and server before replacing files. Back up characters, worlds and the complete Mastery configuration and journals. Install through a compatible mod manager or copy the three supplied plugin components into `BepInEx/plugins`; remove duplicate older copies. Preserve existing configuration rather than replacing it with a new preset.

New profiles use XP ×1. Existing progress and settings are retained. Apex is checked against all 22 level-100 skills: an old 21-skill entitlement does not grant access before Beastmaster 100. Previously tamed animals are retained; mixed historical Farming XP is not blindly reassigned to the new skill.

The optional Comfort Pack adds UI, inventory and building conveniences. Optional item quality, enemy gear drops and weapon specials are off in fresh Core configurations; enable matching rules on each peer if desired. Mastery area storage is optional and disabled by default; external storage and crafting integrations retain their own rules.

## Wiki and support

[Bilingual gameplay wiki: skills, controls, animal husbandry and complete reference tables](https://thunderstore.io/c/valheim/p/ValheimMastery/Valheim_Mastery/wiki/6084-start-bedienung-und-wiki-ubersicht/)

[Report an issue](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/issues/new/choose) with component versions, mod list and reproduction steps. Remove private information from excerpts. See `NOTICE.md` for asset and compatibility notices. **Known limitation:** following animals can remain behind during portal travel. The whistle is a separate recall action with its own safe-arrival checks.

## Deutsch

Valheim Mastery ergänzt **22 Skills** für Kampf, Reisen, Herstellung und Tierhaltung. Jeder Skill hat Meilensteine und ab Level 100 ein Mastery-Cape; alle 22 zusammen schalten das animierte Apex-Cape frei. Slayer-Aufträge, 30 Gebete, Runenmagie und optionale Gegenstandsqualität erweitern den Fortschritt.

Seit 0.18.4: Nixen werden ab Tiermeister 5 zaehmbar und nutzen die bestehenden Futter-, Zucht-, Mutations- und Pflegeregeln. Weitere zahme erwachsene Tiere erhalten Folgen/Warten. Eigene farbige Hitsplashes zeigen Schaden und bestätigte Betäubung ohne geänderte Schadenswerte.

**Tiermeister** verbindet Zähmen, Reiten, Schlachten und Zucht. Freischaltungen reichen vom Wildschwein und Huhn bis zum großen Bergdrachen auf 90. Normale Nachzucht kann sich bis zu vier Sternen verbessern und fällt nicht unter die geerbte natürliche Sternestufe des stärkeren Elternteils. Sterne eins bis vier bleiben gold, fünf Sterne erscheinen pink. Geeignete native Gegnerspawns können fünf Sterne erreichen; festgelegte Gegnerstufen bleiben unverändert.

Maximale Lebenspunkte und absolute native Lebensregeneration gezähmter Tiere steigen mit dem Tiermeister-Level des bekannten Betreuers bis auf das Doppelte bei 100. Paarungsprüfungen erfolgen bis zu doppelt so häufig; Schwangerschaft, Nahrung, Ruhe und Populationsgrenzen gelten weiterhin. Die Mutationschance erreicht bei 100 fünf Prozent. Es sind Zufallswahrscheinlichkeiten, keine garantierten Geburtenzahlen. Hirsch-Zielprüfung und Anzeige akzeptierter Betäubungstreffer sind korrigiert; bestehende Tiere und XP bleiben erhalten.

Rund 30% der wilden erwachsenen Bergdrachen haben dreifache Vanilla-Größe; nur diese sind zähmbar. Schadensfreie Betäubungspfeile benötigen sechs Körper- oder vier Kopftreffer. Danach den gelandeten Drachen füttern. Vorhandene zahme Tiere bleiben zahm, die gespeicherte Größe ändert sich beim Zähmen nicht. Bären- und Drachensättel sind herstellbar.

Aufgesessene Drachen beginnen am Boden. **Springen / Leertaste halten** startet den Flug oder lässt steigen; **Ducken / linke Strg halten** lässt sinken. Geänderte native Tasten werden berücksichtigt, beide gleichzeitig neutralisieren die Höhe. Die konfigurierte **Blocken**-Aktion (Standard rechte Maustaste) fordert eine kontrollierte Landung an. Bei gehaltener Taste unterstützt der Blick die Höhenanforderung zwischen 4,5 und 7,5 m/s um einen Grundwert von 6 m/s. Primärangriff löst alle sechs Sekunden drei Frostgeschosse aus, ohne zusätzliche Angriffsausdauer.

180 Grundausdauer werden mit Tiermeister 100 ohne Cape zu 270. Flug verbraucht 3 pro Sekunde; Start benötigt Folgenstatus, einen geeigneten Untergrund, keine Überlast und mindestens 60% Reserve. Das Tiermeister-Cape ergänzt 20% Kapazität und verdoppelt die Bodenerholung. Rudelbund halbiert 120 Sekunden die eigenen Reitkosten, mit 360 Sekunden Abklingzeit. Der Flug bleibt auf 450 m Radius um den Start und 24 m Höhe über Boden/Wasser begrenzt. Die normale Traglast des Reiters bleibt maßgeblich.

Weitere Systeme sind Schiffreisen zum eigenen Langschiff oder Drakkar, alle 22 Skill-Symbole und die vollständige Meisterschaftsliste. Spezialenergie steht unter der Minikarte, **Umschalt + R** merkt Waffenspezialangriffe vor oder löst die Vormerkung. **C** aktiviert die Cape-Kraft, **Umschalt + C** wählt beim Apex eine Kraft. **Umschalt + T** ruft ab Tiermeister 70 eigene folgende, ungerittene Tiere. Sichere Ankunftsplätze und normale Zugriffsregeln gelten weiterhin.

Die Community-Rangliste umfasst Tiermeister und alle 22 Skills. Anschauen erfordert keine Teilnahme. Erst eine Anmeldung veröffentlicht deinen gewählten Charakternamen, Kategorie und 22 XP-Werte. Es sind selbst gemeldete Werte; Standard und Test/Multiplikator werden getrennt geführt. Du kannst die Teilnahme beenden und das öffentliche Profil löschen. Den Wiederherstellungs-Zugangscode privat aufbewahren. Ältere Einreichungen mit 21 Skills erhalten einen bereits gespeicherten Tiermeisterwert.

Benötigt **BepInExPack_Valheim 5.4.2350** und Valheim **1.0.15, 1.0.16 oder 1.0.17**. **Core 0.18.23, WorldFeatures 1.1.0 und HuntingPhysics 1.0.1** gemeinsam auf Clients und Server installieren. Vor dem Austausch Spiel/Server stoppen und Charaktere, Welten, komplette Mastery-Konfiguration und Journale sichern. Doppelte alte Plugins entfernen; eigene Einstellungen erhalten. Neue Profile starten mit XP ×1.

Apex verlangt alle 22 Skills auf 100; die frühere Berechtigung mit 21 Skills ersetzt Tiermeister nicht. Bestehende zahme Tiere und Fortschritte bleiben erhalten. Alte gemischte Landwirtschafts-XP werden nicht pauschal neu verteilt. Comfort Pack und AzuCraftyBoxes sind optional; Gegenstandsqualität, Ausrüstungsbeute und Waffenspezialangriffe sind in frischen Core-Einstellungen zunächst aus.

Deutsch/englische Anleitungen und Tabellen stehen im Wiki. **Bekannte Einschränkung:** Folgende Tiere können bei Portalreisen zurückbleiben. Der Pfiff ist eine separate Abruffunktion mit eigener Prüfung sicherer Ankunftsplätze. Fehler mit Versionen und nachvollziehbarem Ablauf melden, private Angaben aus Ausschnitten entfernen.

## Übernommene Funktionen aus 0.18.7

- **Report a bug** öffnet im Inventar ein modales Formular für Titel, Beschreibung und optionale Reproduktionsschritte. Mastery- und Spielversion werden sichtbar ergänzt. Erst der eigene Klick öffnet ein vorausgefülltes GitHub-Issue; Prüfung und Versand erfolgen über das eigene GitHub-Konto. Logs, Saves, Spieler-/Weltnamen und Kontodaten werden nicht angehängt. Bericht kopieren dient als lokaler Ausweichweg.
- Wilde und zahme Tiere verwenden Vanilla-Größe und -Position: native Ein-/Zwei-Sternobjekte, passende goldene Sprites für drei/vier und pink für fünf.
- Geeignete wilde Tiere erhalten nach Erreichen von zwei Sternen mindestens 50% pro weiterem Aufstufungswurf. Native Einstiegs-, Distanz-, Feststufen- und Bossregeln gelten weiter. Das bedeutet nicht 50% Fünfsterntiere insgesamt. Bei Tiermeister 100 erhalten normale Nachkommen +2 Rang mit 10%, +1 mit 30%, sonst keinen Bonus; maximal vier Sterne und Schutz der geerbten Stufe bleiben. Bestehende Tiere werden nicht neu ausgewürfelt.
- Acht lokal abschaltbare Herstellungsfilter: Alle, Waffen, Rüstung, Werkzeuge, Munition, Nahrung, Tränke, Sonstiges. Rüstung enthält Schilde, Sonstiges unter anderem Materialien. Native Rezeptliste, Scrollen, Auswahl, Tooltips, Aufwertungsreiter, Materialzahlung und XP bleiben zuständig. Native Mehrfachherstellung und vorhandene Warteschlange ab Level 75 bleiben erhalten: fünf Aufträge, zehn mit Handwerkscape. Keine zweite Queue und keine wählbaren Spezialisierungen. Schalter: `Interface/CraftingCategories`.
- Hochsternbeute steigt moderater: Bei null bis fünf Sternen gelten gewöhnliche Mengenfaktoren 1/2/4/6/8/10 und Chancefaktoren 1/2/4/4/4/4. Trophäen, Quest-/Einzelgegenstände und unbekannte Nicht-Item-Drops bleiben auch in der Menge bei maximal Faktor vier. Native Ausnahmen für unskalierte Drops, Spieleranzahl und Bosse bleiben. Gespeicherte Kadaverbeute und vorhandene XP werden nicht neu berechnet; die Faktoren sind keine pauschale Garantie der erwarteten Gesamtbeute.
- Schilder bieten Text (kein Symbol) oder ein mittiges bekanntes Itemicon. Ausrüstung ist aus neuen Auswahlen ausgeschlossen; gespeicherte Ausrüstungsicons und Text bleiben erhalten. Native Rechteprüfungen und Interface/SignItemIcons bleiben.
- CSV-Escaping und Zusammensetzen der Zeilen laufen im vorhandenen begrenzten Hintergrundschreiber. Unity-Abfragen, Zeitstempel, Reihenfolge und Zahlenformatierung bleiben im Spielthread. Format, Rotation und gezählte Überlast-/Fehlerverluste bleiben erhalten. Kein pauschaler FPS- oder maximaler Speichervorteil wird zugesichert.

Animal Feeding Trough is a separate optional third-party mod. Core support does not install the trough plugin; check the contents of your selected distribution.

Animal Feeding Trough ist eine separate optionale Fremdmod. Die Core-Anbindung installiert die Trogmod nicht; den Umfang der gewählten Distribution prüfen.

# Valheim Mastery 0.18.23 / Installer V111

Built against Valheim 1.0.17. Early magic progression, native interface styling and a targeted QuickStackPlus compatibility fix.

## Deutsch

### Magie

- Neuer früher Stab **Kieselzweig**: ab Magie 6 und Handwerk 1 an der Werkbank. Rezept: 10 Holz, 6 Stein, 4 Harz und 2 Lederreste. Der Stab beginnt mit Kieselstoß; vorhandene gespeicherte Zauberauswahlen bleiben erhalten.
- **Dornwacht** benötigt jetzt vier Hirschfelle statt vier Trollhäuten. Magie-, Handwerk- und Bossvoraussetzungen bleiben erhalten.
- **Runenschmiede** ist als Starterstation bereits mit Baukunst 1 verfügbar. Andere Steinbauten behalten ihre bisherigen Voraussetzungen. Neue Runenschmieden verwenden die vorhandene Starter-Bauvergütung; bereits gespeicherte XP bleiben erhalten.
- Das Magiebuch enthält eine deutsche und englische Einstiegsanleitung zu Stäben, Runenschmiede, Rohlingen, frühen Runen und Grund-Eitr. Die Angaben stammen aus denselben Rezeptdaten wie die Herstellung.
- Eigene überarbeitete Modelle und Inventaricons für Hainfunke, Kieselzweig und Dornwacht, mit Holz, Lederbindungen und gefassten Fokussteinen.
- Runenbeute aus 0.18.22, Eitrvorrat, Regeneration und Endspielwerte bleiben erhalten. Die vorhandenen Leistungsgrenzen einzelner Zauber gelten weiterhin.

### Oberfläche

- Gemeinsame Valheim-nahe Gestaltung für Masteryfenster, Seitenleisten und Hinweise: Holzpanels, Goldakzente und besser lesbare Schriftfarben.
- Skilldetails verwenden passende native Fließtext- und Titelschriften. Die fehlerhafte zusätzliche Abdunklung des Holzpanels wurde entfernt.
- Spezialenergie bleibt unter der Minimap und erhält eine kontrastreiche Textkontur. Hinweise halten Abstand zur geöffneten rechten Seitenleiste; lange Texte und Tooltips werden an den verfügbaren Platz angepasst.
- Überschriften, Magiebuchkarten und Freischaltungshinweise wurden für deutsche und englische Texte verbessert.

### Kompatibilität

- Korrektur der leeren Funktion zum Löschen markierter Gegenstände in der im Windows-Paket verwendeten QuickStackPlus 1.1.2. Die Korrektur greift ausschließlich für die bekannte betroffene Binärdatei.
- Die bestehende typweite Müllmarkierung bleibt erhalten. Löschen erfolgt nur über die ausdrücklich ausgelöste Aktion im geöffneten Inventar; Schnellleiste, Ausrüstung, Questgegenstände und geschützte Slots bleiben ausgenommen. Keine automatische Entsorgung.
- Vorhandener Fortschritt, persönliche Konfigurationen und gespeicherte Gegenstände werden beibehalten. Für Mehrspieler müssen Server und Clients denselben Mastery-Stand verwenden.

## English

### Magic

- Added **Pebble Bough**, an early staff available at Magic 6 and Crafting 1 at the workbench. Recipe: 10 Wood, 6 Stone, 4 Resin and 2 Leather Scraps. It starts with Stone Strike; existing saved spell selections remain authoritative.
- **Thorn Watch** now requires four Deer Hides instead of four Troll Hides. Its skill and boss requirements remain unchanged.
- The **Rune Forge** is available as a starter station at Construction 1. Other stone structures retain their existing requirements. New Rune Forges use the existing starter construction reward; saved XP is preserved.
- Added a German and English spellbook guide covering early staves, the Rune Forge, blanks, early runes and base Eitr. The guide uses the same recipe data as crafting.
- Reworked original models and inventory icons for Grove Spark, Pebble Bough and Thorn Watch, using wood, leather bindings and mounted focus stones.
- Rune drops introduced in 0.18.22, Eitr capacity, regeneration and endgame values remain unchanged. Existing spell-specific power limits still apply.

### Interface

- Unified Mastery windows, side drawers and notifications around native Valheim styling, with wooden panels, gold accents and clearer text colours.
- Skill details now use suitable native body and heading fonts. Removed the additional dark tint incorrectly applied to the wooden background.
- Special energy remains below the minimap and uses a contrasting text outline. Notifications keep clear of the open right drawer; long text and tooltips adapt to the available space.
- Improved headings, spellbook guide cards and unlock notifications for German and English text.

### Compatibility

- Fixed the empty marked-junk deletion routine in QuickStackPlus 1.1.2 included with the Windows package. The compatibility fix applies only to the known affected binary.
- Existing item-type junk markings remain unchanged. Deletion requires an explicit action with the inventory open; hotbar, equipped and quest items and protected slots remain excluded. No automatic disposal.
- Existing progress, personal configuration and saved items are preserved. Multiplayer servers and clients must use the same Mastery version.
