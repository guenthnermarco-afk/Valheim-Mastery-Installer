## Core 0.16.54 / Installer V68 â€” 03 October 2026



- Timed powers for Mining, Woodcutting, Sailing, Slayer, Hunter, Fishing, Construction stamina, Attack, Strength and Agility reserve 240 seconds of active time followed by 360 seconds of cooldown. Attack still refunds only one eligible combo. Death, unequipping and reconnecting do not remove the saved lock; existing old cooldowns are not extended retroactively.
- Magic/field repair keep their three-second channel, home return its separate cooldown, reseeding its toggle, and detection powers their existing timings.
- Construction gains +25 metres at levels 10/30/50/70/90, up to +125 metres. An equipped Construction cape/Apex adds +100 metres. With the native five-metre base this reaches 230 metres, subject to loaded geometry and normal access, distance, station and stability rules; no artificial world loading.
- Reduces repeated HUD cape eligibility checks using a frame-scoped display snapshot. Equipment changes refresh the display and actual activation always validates current eligibility. Controller targets refresh when needed while focus and input ownership checks remain live. No measured in-game FPS gain is claimed.

- Hoe: new Lower ground action uses a 0.5-m target step with a 2-m transition and native depth limits. No resources or XP are generated. A local terrain lattice follows the real terrain vertices; G toggles it while holding the hoe. Clients and server need this Core version.

Hackenbedienung: Im HackenmenÃ¼ â€žBoden absenkenâ€œ wÃ¤hlen. Der Zielpunkt liegt einen halben Meter tiefer; hÃ¶here Nachbarpunkte werden mit weichem Ãœbergang angepasst. Mit G das lokale GelÃ¤nderaster um den Zielpunkt umschalten. Gold markiert ungefÃ¤hr die aktuelle ZielpunkthÃ¶he, Cyan abweichende HÃ¶hen; das ist keine Vorschau der spÃ¤teren Einebnung.

- High Alchemy: select one eligible inventory item in the Magic menu and confirm its displayed coin return. Requires Magic 55 and 20 Eitr; awards 65 base Magic XP with the configured multiplier once, and has a three-second reuse interval. Equipped, quest, custom-data, cheated and unknown items are excluded. Fixed conservative item values do not increase with quality.

Hohe Alchemie: Mit einem passenden Magiestab das Magie-MenÃ¼ Ã¶ffnen, Hohe Alchemie wÃ¤hlen und eine einzelne Umwandlung bestÃ¤tigen. Kosten und MÃ¼nzerlÃ¶s werden vorher angezeigt. Magie55,20Eitr,65Basis-Magie-XP und drei Sekunden Wiederverwendungspause sind die erste Kalibrierung. Kein automatisches Verwerten ganzer Stapel.

- Smithing 20/40/60/80/100 increases smelter and blast-furnace ore/fuel capacity by 20/40/60/80/100 percent. The highest successfully demonstrated filling rank is saved on that station. No automatic filling or change to fuel costs/output.

Schmieden: Ab 20/40/60/80/100 jeweils +20% Erz- und Kohlekapazität, maximal doppelte Grundkapazität. Erfolgreiches Befüllen verbessert den jeweiligen Schmelzofen/Hochofen dauerhaft auf die höchste nachgewiesene Stufe; neue Öfen beginnen unverändert. Kein automatisches Nachfüllen.

- XP balancing: stone XP stays unchanged; copper/tin per-unit base XP becomes2, iron3, silver/obsidian4.5, black metal ore10, black marble17.5 and flametal60.75. Natural resource drops and yield bonuses remain unchanged. One-time taming XP is reduced to20% of its previous value; harvest/slaughter XP and existing earned XP remain unchanged. These are initial corrections from observed sessions, not a verified ten-hour progression claim.

XP-Balancing: Höhere Bergbauressourcen geben weniger XP je tatsächlich erhaltenem Stück; Stein bleibt gleich. Einmalige Zähm-XP auf ein Fünftel reduziert. Bestehende XP, Erträge sowie Ernte- und Schlacht-XP bleiben erhalten.

Deutsch: Die genannten zeitlich begrenzten Cape-KrÃ¤fte erhalten vier Minuten Aktivphase und danach sechs Minuten Abklingzeit. Angriff bleibt eine einzige erstattungsfÃ¤hige Kombo. Bestehende alte SperrstÃ¤nde werden nicht verlÃ¤ngert. Baukunst erhÃ¤lt +25m auf 10/30/50/70/90 und weitere100m durch getragenes Baukunstcape/Apex; maximal230m bei nativer5m-Basis. Es gelten weiterhin geladene Geometrie und native Zugriffs-/Stations-/StabilitÃ¤tsregeln.

Installer V68 retains the V67 comfort mods, settings and MasteryDiagnostics 1.0.0. The optional local performance probe, item-delivery helpers, private encounter modules and the earlier automatic floor-terrain experiment are excluded. Existing progress/settings remain; fresh profiles use XP x1.

## Core 0.16.53 / Installer V67 â€” 03 October 2026

- Tamed animals within five metres of the portal can accompany a completed player portal trip when their network object is confirmed to be locally owned. Wolves must be following that exact player. The same animal/ZDO is moved; animals are not cloned or replaced.
- Travel requires a loaded destination and a safe free landing position. Dead/wild animals, ridden or attached animals and animals behind a closed wall are excluded. Cancelled trips move nothing. Remote-owned animals or ownership changes leave animals at the origin; remote-owner transport is not guaranteed.
- Reduces repeated allocations in Prayer updates and cape inventory checks. XP HUD text is refreshed when its displayed state changes. No measured FPS gain is claimed.

Deutsch: GezÃ¤hmte Tiere im Umkreis von fÃ¼nf Metern um das betretene Portal kÃ¶nnen nach abgeschlossener Reise folgen, sofern ihr Netzwerkobjekt weiterhin bestÃ¤tigt lokal verwaltet wird. WÃ¶lfe mÃ¼ssen genau dem reisenden Spieler folgen. Derselbe Tier-ZDO bleibt erhalten; keine Kopien. Das Ziel muss geladen sein und einen sicheren freien Landeplatz bieten. Fremdverwaltete Tiere und Tiere mit Besitzwechsel bleiben zurÃ¼ck. Abgebrochene Reisen verschieben nichts. Reduzierte wiederholte Speicherallokationen bei Gebet/Cape-PrÃ¼fungen und bedarfsgerechte XP-HUD-Texte; kein versprochener oder bereits gemessener FPS-Gewinn.

Targeted native/policy checks, independent reviews and the release build passed. Actual portal gameplay, sector-unload ownership transitions and multiplayer travel remain unverified in game. This is deliberately conservative local-owner support, not a complete remote-owner transport protocol.

Installer V67 retains the same comfort mods and MasteryDiagnostics 1.0.0 as V66. No local hotpath probe, personal item helper, private encounter module or terrain experiment is included. Existing progress/settings remain; new profiles use XP x1. Update clients and server together.

## Core 0.16.52 / Installer V66 â€” 03 October 2026

- Combat-style tooltips omit zero-valued bonuses.
- Skillcape cooldowns use the native status bar and their matching icons.
- The Prayer bar shows continuous remaining points and updates immediately.
- Both Prayer drink icons use the native round corked bottle with cyan liquid, preserving the original cork, shading and transparency.
- Prayer Potion restores 60 points; Prayer Mead remains at 20. Recipes and drinking cooldowns are unchanged.

Deutsch: Kampfhaltungen zeigen keine wirkungslosen Nullboni mehr. Skillcape-Abklingzeiten erscheinen mit passenden Symbolen in der nativen Statusleiste. Der Gebetsbalken zeigt den verbleibenden Vorrat stufenlos und aktualisiert sofort. Beide GebetsgetrÃ¤nke erhalten native runde Flaschenicons mit cyanfarbenem Inhalt; Korken, Schattierung und Transparenz bleiben erhalten. Der Gebetstrank stellt 60 Punkte wieder her, Gebetsmet weiterhin 20; Rezepte und Trinkpausen bleiben gleich.

Installer V66 retains the same comfort mods and MasteryDiagnostics 1.0.0 as V65. No personal delivery helpers, private encounter modules or terrain experiments are included. Existing progress and settings remain; fresh profiles use XP x1. Update Core on clients and server together.

Targeted regression checks, independent code review and the release build passed. No new background game was launched for this release.

## 0.16.51 / Installer V65 â€” 03 October 2026

- Mining XP now covers the native small-stone, tin and obsidian drop paths, including legitimate zero-weight stone drops; awards remain based on actual resources.
- Redesigned magic staves and prestige Slayer helmets; inherited staff effects removed. The Prayer HUD icon below its bar now scales with the bar width.
- Mastery and Max capes hang on native wall stands with a rolled cloth edge, without the worn collar or clasps. All eight Max Cape styles remain available.
- Construction 100 recovers paid initial recipe ingredients previously excluded from manual demolition refunds. Free saved materials, later-added fuel and consumed feast portions are not duplicated; ordinary native refunds and XP remain unchanged.
- Combat level uses Attack, Strength, Defence, Hitpoints and Prayer, capped at 126. Equipment, Ranged and Magic are excluded; progress is not reset. Native skill title and optional BetterUI display agree.
- Installer V65 retains the optional client-side local diagnostics from V64. No private modules or personal item-delivery helpers are included.

Deutsch: Bergbau-XP fuer Stein/Zinn/Obsidian korrigiert; neue Stab- und Prestigehelmgestaltung sowie ein mit der Balkenbreite skaliertes Gebets-HUD-Symbol unter dem Balken. Wandcapes ohne Kragen, mit eingerolltem Stoffrand und acht Max-Cape-Stilen. Baukunst 100 erstattet bezahlte Anfangszutaten beim manuellen Abriss, ohne kostenlose Materialien oder nachgefuellten Brennstoff zu vermehren. Kampfstufe aus Angriff, Staerke, Verteidigung, Lebenspunkten und Gebet bis 126; vorhandene XP bleiben erhalten. Clients und Server gemeinsam aktualisieren. Bestehende Einstellungen bleiben, neue Profile starten mit XP x1.

Validation: targeted source/native contracts, release build and independent review passed. Visual feedback was incorporated during test play; this is not a claim that every multiplayer edge case has been reproduced.

# Valheim Mastery â€” Public Beta

## Changes since 0.16.48 / Ã„nderungen seit 0.16.48

- **Attack cancellation:** use your configured block or dodge input to interrupt melee, ranged and magic attacks. Already spent resources are not refunded, launched projectiles remain active, and interrupted combos do not earn the combo refund.
- **Production and Slayer XP:** cooking, fermentation and smelting identify remote players through network character data. Separate host/world receipts prevent stale copied worlds from suppressing new credits or replaying historical production. Slayer boards accept lower historical server snapshots without duplicating XP or marks.
- **Prayer:** withered bones can be offered for 1,500 base Prayer XP; successful offerings are included in XP telemetry.
- Update all clients and the server together. Existing progress remains; missing historical XP is not automatically repaid.

- **Angriffe abbrechen:** die eingestellte Block- oder Ausweicheingabe unterbricht Nahkampf-, Fernkampf- und Magieangriffe. Bereits bezahlte Ressourcen werden nicht erstattet; gestartete Projektile bleiben wirksam. Abgebrochene Kombos erhalten keine Kombo-Erstattung.
- **Produktions- und Slayer-XP:** Kochen, Fermentieren und Schmelzen ordnen entfernte Spieler anhand ihrer Netzwerk-Charakterdaten zu. Getrennte Host-/Welt-Belege verhindern, dass alte Weltkopien neue Gutschriften verschlucken oder frÃ¼here Produktionen erneut auszahlen. Slayer-Bretter verarbeiten Ã¤ltere ServerstÃ¤nde ohne doppelte XP oder Marken.
- **Gebet:** verdorrte Knochen geben als Opfer 1.500 Basis-Gebets-XP; erfolgreiche Opfer werden in der XP-Telemetrie erfasst.
- Clients und Server gemeinsam aktualisieren. Bestehender Fortschritt bleibt erhalten; fehlende historische XP werden nicht pauschal nachgezahlt.

### Known validation limits / PrÃ¼fgrenzen

Cooking, Alchemy and smelting credits have been confirmed in live play after the XP fix. Attack cancellation has passed build and assembly-contract checks; actual animation transitions and multiplayer acceptance are still pending. The earlier remote-owner combo/refund proof remains outstanding. No universal performance or leveling-time guarantee is made.

Koch-, Alchemie- und Schmelzgutschriften sind nach dem XP-Fix im laufenden Spiel bestÃ¤tigt. AngriffsabbrÃ¼che haben Build- und Assembly-VertragsprÃ¼fungen bestanden; die praktische Animations- und Mehrspielerabnahme steht noch aus. Der frÃ¼here Remote-Kombo-Nachweis bleibt offen. Keine allgemeine Leistungs- oder Levelzeitgarantie.

**Version 0.16.53 Â· 21 connected skills including Prayer. A new combat progression. Slayer contracts. Mastery Capes.**

Inspired by **Old School RuneScape (OSRS)**: level-based progression, mastery capes,
Slayer contracts and long-term mastery, adapted to Valheim's survival and co-op
gameplay. Valheim Mastery is an independent fan-made mod, not affiliated with or
endorsed by Jagex.

Build a character through combat, gathering, production and exploration. Every
Mastery skill progresses from level 1 to 100, with unlocks, milestones and a
dedicated Mastery Cape. The Apex Mastery Cape combines all Mastery Cape bonuses after mastering
all twenty-one skills at level 100. Existing Apex owners retain their grandfathered entitlement.

This is an early public beta with **German and English** gameplay text. Mastery
follows Valheim's language setting; other languages currently use English.

Quick prayers: save up to three compatible unlocked prayers in the Prayer panel, then switch the set together. Blue highlighting marks active effects. Combat, protection and regeneration prayers consume more points; active prayers persist through dungeon and portal transitions.

## What is included?

| Area | Skills |
| --- | --- |
| Combat | Attack, Strength, Defence, Hitpoints, Ranged, Magic |
| Gathering and wildlife | Mining, Woodcutting, Foraging, Hunter, Fishing |
| Production | Smithing, Crafting, Farming, Cooking, Alchemy |
| Exploration and building | Agility, Sailing, Construction |
| Contracts | Slayer |
| Prayer | Prayer |

- Combat styles, accuracy, max hits and equipment requirements. Accuracy failures
  become 25% glancing hits; successful parries remain damage-free. Immunities and
  arrows that physically miss are separate from accuracy rolls.
- Optional Vanilla equipment itemization: persistent crafted and dropped quality with matching
  weapon, armor, shield and cape bonuses, including six elemental staves.
  Unique and decorative items keep their separate equipment rules.
  Native set bonuses, resistances, elemental effects and summons are preserved.
- Optional NPC gear loot: a curated set of ordinary enemies can leave at most one extra
  equipment item from their progression tier, with stored quality and a chance
  of an affix. Starred enemies improve the loot chance and quality. Native
  material and trophy drops remain available; bosses and special reward sources
  use their own rules. Tamed, bred and player-summoned creatures are excluded.
- Optional **Dyrnwyn Perfect Strike**: arm the next eligible attack using the SP
  button. A committed attack costs 50 of a maximum 100 Special Energy and adds an accuracy boost with
  an optional short fire visual. Dyrnwyn is the only Special weapon in this release. The compact bar appears only with a supported equipped weapon and stays
  visible at zero energy. See activation instructions below.
- Base stamina, health and Eitr progression; movement and swimming through Agility.
- Resource tiers, production milestones, material-saving chances, farming grids,
  additional cultivatable plants and natural ore/tree regeneration.
- Hunter carcass processing and lethal baited traps. Bait attracts nearby wild
  boars and hares within 18 metres; the trap springs on contact.
- Slayer contracts, two-player shared tasks, completion and streak tokens,
  prestige upgrades, reward crates, weapons and unlockable Monsterbane headgear styles.
  The three main helmet tiers and their nine color variants share the revised
  Slayer silhouette, with recessed eye channels and bone-to-metal materials.
- A Runebound Staff with four Eitr-powered Barrage spells and area effects.
- Twenty-one Mastery Capes and eight styles of the animated Apex Mastery Cape.
- Prayer progression with 30 prayers, a buildable altar, trophy and bone-fragment offerings, and Prayer Mead. The Prayer panel is ordered by unlock level, shows each Prayer's bonus and point drain, and accepts touch and controller input. Active Prayer icons show the same details in their status-bar tooltip. The mead base uses the existing cauldron and fermenter; no extra brewing station is needed.
- Collapsible screen-edge tabs for Prayer, Magic, combat styles and senses, with touch and controller input. A successful selection closes its panel. Hold the HUD cursor key to select with the mouse; conflicting game bindings must be reassigned. The vanilla status bar also displays the current combat style, active prayers and sense cooldowns.
- Freeform Construction, building-area projects, work orders and area repair.
  At level 100, the equipped Construction cape also offers **Return home** to
  your own bed set as your respawn point in this world. Alt+F1 with a hammer,
  or the Construction board button, opens the choice. Area repair remains;
  each power has its own 6-minute cooldown. Normal world and inventory transport
  rules apply. Without a valid selected bed, return home is unavailable.
  **Prebuilt village blueprints are temporarily disabled.** Saved plans remain
  dormant; already built pieces are preserved.
- The basic campfire is buildable at Construction 1. With BetterUI installed,
  enable its `customSkillUI` setting; Mastery then displays its twenty-one skills
  in that renderer. The optional Comfort Pack includes this setting.

## Install

1. Use a fresh Valheim profile in a Thunderstore-compatible mod manager.
2. Install this package and its declared BepInEx dependency, then launch modded.
3. For the first beta session, use a new character and test world, or back up your
   character, world and existing mod configuration before loading them.
4. Open the skill window and click a Mastery skill to inspect its milestones.

Built against **Windows / Steam Valheim 1.0.16**, using
**BepInExPack_Valheim 5.4.2350**. The plugin also accepts 1.0.15.
Other operating systems are unverified. See the beta limitations below.

The core mod does not require BetterUI, Jotunn or Equipment and Quick Slots.
With Equipment and Quick Slots, the quiver can use additional inventory cells.
Without it, equip the quiver by right-clicking it; ammunition stays in the main
inventory.

For manual installation, install BepInEx separately and copy this archive's
`plugins/ValheimMastery/` folder into `BepInEx/plugins/`.

## Progression and configuration

Fresh installations use **XP x1**. All twenty-one skills share the same thresholds:
level 100 requires **1,439,116 XP**. Approximately 10 hours of relevant activity
per skill is a balancing target, not a measured completion-time guarantee.

Standard progression uses XP x1. Existing custom multipliers and earned progress are preserved. Higher multipliers deliberately accelerate progression.
Hitpoints awards are 30% of awarded primary combat XP, including block/parry
Defence XP. These are balancing changes, not a measured ten-hour completion guarantee.

After the first launch, close the game and edit
`BepInEx/config/org.valheim.mastery.cfg`:

```ini
[Progression]
CombatXpMultiplier = 1
```

Despite its historical name, this setting controls all Mastery skills and the
integrated native/mod skill XP paths. For faster progression, set it to `5`.
The host controls the multiplayer multiplier. Existing settings are not replaced
by this package. The development XP slider is not included in this release.

### Enable itemization and Dyrnwyn Perfect Strike

The Thunderstore Core and Comfort packages preserve existing Mastery settings.
On a fresh profile, the new itemization and Special options are **off by default**.
After the first launch, close Valheim and set the following keys in
`BepInEx/config/org.valheim.mastery.cfg`, keeping the other settings intact.
You can also edit these keys with a compatible configuration manager.

```ini
[Prototype]
EnableItemizationI01I04 = true
EnableItemizationEarlyVanilla = true
EnableItemizationMidVanilla = true
EnableItemizationLateVanilla = true
EnableItemizationEndgameVanilla = true
EnableItemizationDefenceVanilla = true
EnableItemizationDirectMagicVanilla = true
EnableNpcGearDrops = true

[Special Attacks]
EnableSpecialAttacks = true
EnableSpecialVisual = true
```

Use the same Mastery version and gameplay settings on every client and the host
or dedicated server, then restart them. Connections with different Mastery
versions or combat rules are rejected. The visual switch is local and does not
have to match; the host supplies the XP multiplier.

Existing ordinary gear remains neutral, including when upgraded. Newly crafted
supported equipment and new eligible NPC gear drops receive an itemization
identity; upgrading an item that
already has an identity preserves its stored quality. No new keys are assigned
automatically: use the SP button through the existing HUD cursor, or configure the optional `ArmKey` or `QuickUseModifier`
after checking your bindings. The modifier works with your existing primary attack.

`EnableNpcGearDrops` requires the core itemization switch and the switches for
the equipment groups you want in the loot pools. It is off on fresh profiles.
Changing this setting does not reroll existing items or previous deaths.
Generated gear keeps its stored quality when picked up, transferred or loaded.
The curated list does not cover every creature. Loot pools follow the source creature: for example, trolls can yield troll
equipment and draugr can yield iron equipment. These are occasional bonus drops.
The current base chance ranges from 1.5% to 6.05%, depending on tier and stars;
the separate affix chance applies only after an equipment drop succeeds.

Anonymous balancing telemetry is stored locally under
`BepInEx/ValheimMastery/balancing`. It records XP sources, active-time windows,
outputs, perk procs and resource/combat samples; multipliers are normalized back
to x1 for comparison. It does not transmit data or record player/world names,
chat, peer IDs or coordinates. Set `Diagnostics.EnableBalanceTelemetry = false`
to disable future recording.

Existing Mastery progress is retained. Compatible existing vanilla and legacy
mod skill levels are imported once where a matching migration exists;
new skills begin at level 1. Loading an existing character can perform that
migration, so make the backup **before** the first Mastery session.

## Character backups and recovery

Mastery automatically keeps a local backup after a healthy character save.
It covers all 21 Mastery skill progressions and their character unlocks, plus
Mastery items and equipment with Mastery quality actually held in the character
inventory. Item quality and saved properties are retained. Equipped items and
Equipment and Quick Slots 3.1.3, including the Mastery quiver, are supported.
World chests, graves and separate bag inventories are not included.

If the next healthy load finds a missing or lower saved state, a recovery prompt
appears before the old backup is replaced. You can also open **Mastery recovery**
from the inventory. Review the listed skills and items, then choose:

- **Review recovery** and **Confirm loss and recover** to restore the listed state.
  Make room in the ordinary inventory first; recovered items are not auto-equipped.
- **Keep current state** to accept what the character currently has.
- **Later / close** to keep the previous evidence and decide another time.

Nothing is restored automatically. A backup cannot observe transfers, consumption
or deaths while Mastery is absent. Missing items may still exist in a chest,
grave or another player's inventory; confirming recovery could duplicate them.
A first backup cannot recreate items lost before the backup existed. Already
spent resources, claimed rewards and world-side Slayer accounts are not rolled back.
An interrupted confirmed recovery remains blocked for manual review instead of
issuing the same items again. Keep its files; do not delete them to force a retry.

Use **Show backup folder** in the recovery window to find the character's files.
They live under `MasteryRecovery` in the active Valheim save directory and are
**not automatically synchronized by Steam Cloud**. Copy the complete recovery
folder along with character saves when moving to another device. A change between
local and cloud save sources requires review. Continue keeping full character
and world backups separately.

## Controls

| Key | Action |
| --- | --- |
| F1 | Cycle combat style |
| Q | Activate the selected sense |
| F2 | Cycle resource, contract, hunting and fishing senses |
| Shift + F2 | Native connection information |
| B | Toggle saved compatible Quick Prayers; disabled with building tools |
| F4 | Cycle unlocked rune-focus spells |
| F5 | Open rune spellbook |
| F3 | Cycle unlocked Runebound Staff spells |
| Hold R | Use the HUD cursor to choose a combat style, sense or prayer; move Valheim's Hide action to T first |
| Controller view button + shoulder buttons | Navigate the combat-style and sense HUD; south face button activates the focused choice |
| Controller view button + D-pad up/down | Navigate the Prayer list; east face button toggles the focused prayer |
| Touch the left PRAYER / GEBET tab | Open or close the Prayer list |
| Hold R and click SP | Arm or cancel Dyrnwyn Perfect Strike; then use the normal primary attack |
| Hold middle mouse | Bow/crossbow zoom |
| Ctrl + F1 | Slayer Mastery Cape berserk |
| Shift + F1 | Contextual Mining, Woodcutting or Sailing power |
| Alt + F1 | Contextual Hunter, Construction or Fishing cape power |
| Alt + Q | Slayer hunting instinct, when unlocked |

Controls are configurable. The Apex Mastery Cape keeps the same contextual controls;
Q activates only the selected sense. Auto-run is unbound by the mod.
The SP button also accepts touch and HUD controller focus when Special attacks
are enabled. Controller button labels depend on the selected device layout.

### Additional usage / Weitere Bedienung

Hold R, then click the Prayer, Magic, Style, Senses, Mastery or Apex tab. R frees the cursor; it does not automatically open a panel. If bindings conflict, move Hide weapon to T and the emote wheel to Y, or select another HUD key. Successful selections close panels. B toggles the saved prayer set; blue rows show actual active prayers, checkboxes only saved selections. Shift+F3 selects the previous Runebound spell.

R halten und Gebet, Magie, Stil, Sinne, Mastery oder Apex anklicken. R gibt die Maus frei, Ã¶ffnet aber nicht automatisch ein Fenster. Bei Konflikten Waffe wegstecken auf T und Emote-Rad auf Y oder eine andere HUD-Taste wÃ¤hlen. B schaltet gespeicherte Schnellgebete; blaue Zeilen zeigen aktive Gebete, HÃ¤kchen gespeicherte Auswahl. F4 wechselt Runenfokus-Zauber, F5 Ã¶ffnet das Zauberbuch; Umschalt+F3 wechselt rÃ¼ckwÃ¤rts.

| Input / Eingabe | Action / Aktion |
| --- | --- |
| Shift+Use / Umschalt+Benutzen | Cooking station: one paid batch, limited by available slots / Kochstation: eine bezahlte Charge mit freien PlÃ¤tzen |
| Ctrl+Shift+Use / Strg+Umschalt+Benutzen | Cooking 75: up to five batch orders / Kochen 75: bis zu fÃ¼nf ChargenauftrÃ¤ge |
| Shift+Use / Umschalt+Benutzen | Own fermenter, Alchemy 90: batch planner / Eigener Fermenter, Alchemie 90: Chargenplaner |

Mastery directly activates an eligible individual cape power; Construction offers two actions and Apex lists eligible powers. Field repair opens inventory selection and requires 3 seconds stationary,10 seconds out of combat and one explicit recipe metal. Production queues are selected in the crafting inventory and check/pay every order separately, respecting native maximum quality. Optional Farming resowing is toggled through Mastery/Apex and requires cultivator, seed payment and recorded own planting provenance. Foraging filters and Sailing target pins are in skill details; the Construction board shows own-piece condition.

Mastery aktiviert eine berechtigte Einzelcape-Kraft, Baukunst bietet zwei Aktionen, Apex die verfÃ¼gbaren KrÃ¤fte. Feldreparatur Ã¶ffnet die Inventarauswahl:3 Sekunden still,10 Sekunden kampffrei und ein Hauptmetall aus dem Rezept. Herstellungsfolgen werden im Herstellungsinventar gewÃ¤hlt; jeder Auftrag wird einzeln geprÃ¼ft und bezahlt, native MaximalqualitÃ¤t gilt. Nachsaat Ã¼ber Mastery/Apex benÃ¶tigt Kultivator, Saatgut und erfasste eigene Pflanzherkunft. Sammlerfilter und Segelziel stehen in Skilldetails, Bauzustand am Baubrett.

F6â€“F8 quickslots and F10 BetterUI editing are optional comfort-mod bindings, not Core controls. / F6â€“F8-Schnellslots und F10-BetterUI-Bearbeitung gehÃ¶ren zu optionalen Komfortmods, nicht zum Core.

### Host identity backup / HostidentitÃ¤t sichern

Also preserve `BepInEx/ValheimMastery/combat-host-identity-v2.txt` together with the host journals and world backups. Do not delete or regenerate it to reset XP. Copying an entire installation including this identity intentionally retains the same authority; a separate installation receives a separate identity. Character/journal rollback needs an explicit recovery review and does not automatically rebase checkpoints.

ZusÃ¤tzlich `BepInEx/ValheimMastery/combat-host-identity-v2.txt` mit Hostjournalen und Welt sichern. Nicht als XP-Reset lÃ¶schen oder neu erzeugen. Eine vollstÃ¤ndig kopierte Installation einschlieÃŸlich IdentitÃ¤t bleibt absichtlich dieselbe Instanz; eine separate Installation erhÃ¤lt eine eigene IdentitÃ¤t. Charakter-/Journal-Rollback setzt Checkpoints nicht automatisch zurÃ¼ck.

## Multiplayer beta

Every player and the host or dedicated server must use the same Mastery release
and matching combat, itemization and Special gameplay settings. Visual effects
and keybindings may differ. Use a compatible Valheim version on each machine.

Slayer co-op is explicitly started for two players at the board. Join before
the first kill; qualifying nearby participants receive the same Slayer kill XP.
Tokens are awarded at completion. Both players must be alive and within the
required 70 m completion range to receive the shared completion reward.

Multiplayer remains a beta feature, particularly reconnects, ownership changes
and long sessions. Dedicated-server support is experimental.

Back up `BepInEx/config/ValheimMastery/` alongside character and world saves.
This directory contains the host's `slayer-<world-id>.json` ledger and
`combat-coop-<world-id>.tsv` combat-credit journal. Replacing the DLL does not
reset them. If an interrupted journal write can be recovered, Mastery saves a
`.recovery-*.bak` copy first. Corruption in completed records or an ambiguous
legacy tail stops shared combat credits and is reported in the log; do not
delete the journal to force a reset.
Older Mastery releases cannot read the new checksummed journal entries. Before
updating, keep a backup of this directory; reverting the DLL alone is insufficient
for a downgrade. Restore a matching journal backup if returning to an older release.

## Compatibility and updates

Do not run the replaced Smoothbrain Mining, Lumberjacking, Blacksmithing,
Farming, Foraging, Cooking or Sailing plugins alongside Mastery. Their known
plugin IDs are declared incompatible. Back up first, then disable those plugins;
Mastery can read supported legacy progress without their DLLs being loaded.

BetterArchery, other combat overhauls, additional skill-replacement plugins and
SkillBonusTooltips are outside the supported starting setup. Begin with the core
mod and add optional UI/comfort mods only after it works.

Close Valheim before updating. If Mastery cannot initialize, it disables its
startup and cleans up its own patches and components. Check
`BepInEx/LogOutput.log`, resolve the reported cause and restart the game.

Do not load the same character in a vanilla
session as an uninstall test: this mod adds saved progress, items and world
objects. Restore a pre-Mastery backup for a clean rollback.

## Known limits

- Village blueprint placement and terrain preparation are intentionally paused.
- Bait attracts boars and hares only. Birds can still trigger a baited trap
  when they land on it, but are not drawn toward it.
- Languages other than German and English currently fall back to English.
- The 10-hour progression target needs real playtime feedback.
- Multiplayer reconnects, long sessions and dedicated servers remain experimental.
- Controller layouts may need rebinding; complete controller support and all
  Prayer-effect combinations remain under development.
- Third-party enemy/content mods may need explicit compatibility work.
- Reducing damage to zero does not remove status effects that are already active.

## Useful beta feedback

**[Report a bug or balance problem on GitHub Issues](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/issues/new/choose).**
This is the feedback channel for both the standalone mod and Comfort Pack.
Public reports are visible to other users, so remove personal information.

Include the Mastery and Valheim versions, XP multiplier, installed mods, whether
you were host/client, exact reproduction steps and expected/actual behaviour.
For balance feedback, add your skill level, activity and rough duration.

Attach only the relevant log excerpt from `BepInEx/LogOutput.log`; remove
private server details and personal paths first. `FEEDBACK.md` contains a template.

Unofficial fan-made mod. Not affiliated with Iron Gate, Coffee Stain or Jagex.
See `NOTICE.md` for asset and compatibility attribution.

## Deutsch

**Valheim Mastery 0.16.51** ist eine Ã¶ffentliche Beta mit 21 Fertigkeiten,
Stufen von 1 bis 100, Slayer-AuftrÃ¤gen und Mastery Capes. Inspiriert von
Old School RuneScape (OSRS), angepasst an Valheims Ãœberleben und Koop-Spiel.
Die Spieltexte folgen Valheims Sprache: Deutsch oder Englisch; andere Sprachen
verwenden derzeit Englisch. Dieses unabhÃ¤ngige Fanprojekt ist nicht mit Jagex,
Iron Gate oder Coffee Stain verbunden und wird von ihnen nicht unterstÃ¼tzt.

### Inhalte

| Bereich | Fertigkeiten |
| --- | --- |
| Kampf | Angriff, StÃ¤rke, Verteidigung, Lebenspunkte, Fernkampf, Magie |
| Sammeln und Tiere | Bergbau, HolzfÃ¤llen, Sammeln, Jagd, Angeln |
| Herstellung | Schmieden, Handwerk, Landwirtschaft, Kochen, Alchemie |
| Erkundung und Bauen | Gewandtheit, Segeln, Baukunst |
| Weitere | Slayer, Gebet |

- Kampfstile, Genauigkeit, maximaler Schaden und AusrÃ¼stungsanforderungen.
  Misslungene GenauigkeitswÃ¼rfe verursachen Streiftreffer mit 25 % Schaden;
  erfolgreiche Paraden bleiben schadensfrei. ImmunitÃ¤ten und tatsÃ¤chlich
  vorbeifliegende Geschosse sind davon getrennt.
- Optionale Itemization fÃ¼r unterstÃ¼tzte Vanilla-Waffen, RÃ¼stungen, Schilde,
  Capes und sechs ElementarstÃ¤be: gespeicherte Herstellungs-/BeutequalitÃ¤t und passende
  AusrÃ¼stungsboni. Einzigartige und dekorative GegenstÃ¤nde behalten ihre eigenen
  Regeln. Native Setboni, Resistenzen, Elementareffekte und BeschwÃ¶rungen bleiben.
- Optionale NPC-AusrÃ¼stungsbeute: eine kuratierte Auswahl gewÃ¶hnlicher Gegner kann hÃ¶chstens
  ein zusÃ¤tzliches AusrÃ¼stungsteil ihrer Fortschrittsstufe hinterlassen, mit
  gespeicherter QualitÃ¤t und einer Chance auf ein Affix. Sterne erhÃ¶hen die
  Beutechance und QualitÃ¤t. Native Materialien und TrophÃ¤en bleiben erhalten;
  Bosse und besondere Belohnungsquellen haben eigene Regeln. GezÃ¤hmte,
  gezÃ¼chtete und vom Spieler beschworene Kreaturen sind ausgeschlossen.
- Dyrnwyns optionaler **Perfect Strike** verbraucht 50 von maximal 100
  Spezialenergie und verbessert die Treffergenauigkeit. Der kurze Feuereffekt
  ist rein optisch. Nur Dyrnwyn hat derzeit ein eigenes Special. Die kompakte
  Spezialleiste samt SP erscheint nur mit einer passenden ausgerÃ¼steten Waffe
  und bleibt dann auch bei 0 Energie sichtbar.
- Fortschritt fÃ¼r Leben, Ausdauer und Eitr; Bewegung und Schwimmen Ã¼ber Gewandtheit.
  Rohstoffstufen, Herstellungsmeilensteine, Materialersparnis, Pflanzraster,
  zusÃ¤tzliche Nutzpflanzen und Regeneration natÃ¼rlicher Erze und BÃ¤ume.
- Jagd mit Kadavern und tÃ¶dlichen KÃ¶derfallen. Die Fallen locken wilde
  Wildschweine und Hasen aus bis zu 18 m an und lÃ¶sen bei BerÃ¼hrung aus.
- Slayer-AuftrÃ¤ge, gemeinsame Zweispieler-AuftrÃ¤ge, Abschluss- und Serienmarken,
  Prestige, Belohnungskisten und Waffen. Drei Ã¼berarbeitete Slayerhelm-Stufen
  mit neun zusÃ¤tzlichen Farbvarianten und innenliegenden AugenkanÃ¤len.
- Runebound Staff mit vier Eitr-basierten Barrage-Zaubern und FlÃ¤chenwirkungen.
- 21 Fertigkeitscapes sowie acht Stile des animierten Apex Mastery Cape.
  Neue Apex-Freischaltungen benÃ¶tigen alle 21 Fertigkeiten auf Stufe 100;
  bereits gespeicherte Ã¤ltere Berechtigungen bleiben erhalten.
- Gebet mit 30 Gebeten, Altar, TrophÃ¤en- und Knochenopfern sowie Gebetsmet.
  Die Liste zeigt Freischaltstufe, Wirkung und Punkteverbrauch. Metbasis und
  Met verwenden Kessel und Fermentierer; eine zusÃ¤tzliche Station ist unnÃ¶tig.
- Kampfstil- und Ortungs-HUD mit Maus-, Touch- und Controllerbedienung.
  Die Statusleiste zeigt Kampfstil, aktive Gebete und Ortungs-Abklingzeiten.
- Freie Baukunst, Baugebiete, AuftrÃ¤ge und FlÃ¤chenreparatur. Ab Level 100 bietet
  das ausgerÃ¼stete Baukunstcape zusÃ¤tzlich **Heimkehr** zum eigenen Bett, das in
  dieser Welt als Respawnpunkt gesetzt ist. Alt+F1 mit Hammer oder
  der Knopf am Baubrett Ã¶ffnet die Auswahl. Gebietsreparatur bleibt erhalten;
  beide KrÃ¤fte haben eigene sechs Minuten Abklingzeit. Die normalen Welt- und
  Inventartransportregeln gelten. Ohne gÃ¼ltiges gesetztes Bett keine Heimkehr.
  Dorf-BauplÃ¤ne sind
  vorÃ¼bergehend deaktiviert; gespeicherte PlÃ¤ne und bereits gebaute Teile bleiben.
  Das einfache Lagerfeuer ist ab Baukunst 1 verfÃ¼gbar.

### Installation und Fortschritt

1. Ein frisches Profil in einem Thunderstore-kompatiblen Modmanager verwenden.
2. Dieses Paket samt BepInEx-AbhÃ¤ngigkeit installieren und modifiziert starten.
3. Vor dem ersten Laden bestehende Charaktere, Welten und Konfigurationen sichern;
   alternativ einen neuen Charakter und eine neue Welt verwenden.
4. Im Fertigkeitsfenster eine Fertigkeit anklicken, um ihre Meilensteine zu sehen.

Zielversion ist Windows/Steam-Valheim **1.0.16** mit BepInExPack_Valheim
**5.4.2350**; 1.0.15 wird ebenfalls akzeptiert. Andere Betriebssysteme sind
ungeprÃ¼ft. Zur manuellen Installation BepInEx separat installieren und
`plugins/ValheimMastery/` nach `BepInEx/plugins/` kopieren.

BetterUI, Jotunn und Equipment and Quick Slots sind fÃ¼r den Core nicht nÃ¶tig.
Mit Equipment and Quick Slots kann der KÃ¶cher zusÃ¤tzliche Inventarfelder nutzen.
Ohne diese Mod den KÃ¶cher per Rechtsklick ausrÃ¼sten; Munition bleibt im Hauptinventar.
Bei BetterUI `customSkillUI = true` verwenden, damit alle 21 Fertigkeiten angezeigt
werden. Das optionale Komfortpaket liefert diese Einstellung mit.

Frische Profile verwenden **XP Ã—1**. Alle 21 Fertigkeiten teilen dieselben
Schwellen; Stufe 100 benÃ¶tigt **1.439.116 XP**. Etwa zehn Stunden sinnvoller
TÃ¤tigkeit je Fertigkeit sind ein Balancingziel, keine zugesicherte Spielzeit.
Nach dem ersten Start Valheim schlieÃŸen und bei Bedarf in
`BepInEx/config/org.valheim.mastery.cfg` unter `[Progression]` den Wert
`CombatXpMultiplier = 1` anpassen, etwa auf `5` fÃ¼r schnelleren Fortschritt.
Der Wert betrifft trotz seines Namens alle Mastery-Fertigkeiten und eingebundene
native beziehungsweise Mod-XP-Pfade. Im Multiplayer gilt der Wert des Hosts.
Vorhandene Einstellungen werden durch das Paket nicht ersetzt.

Bestehender Mastery-Fortschritt bleibt gespeichert. UnterstÃ¼tzte Vanilla- und
Ã¤ltere Mod-Fertigkeitsstufen werden einmalig Ã¼bernommen; neue Fertigkeiten starten
bei 1. Die Ãœbernahme kann beim ersten Laden stattfinden, deshalb vorher sichern.

### Itemization und Spezialangriff aktivieren

Beide Funktionen sind in frischen Profilen zunÃ¤chst ausgeschaltet. Nach dem
Beenden des Spiels die **acht Itemization- und zwei Special-EintrÃ¤ge im obigen
Configblock** auf `true` setzen. Alle anderen Werte erhalten. Dasselbe Mastery-
Release und dieselben Spielregeln auf Clients und Host beziehungsweise Server
verwenden und alle neu starten. Abweichende Versionen oder Kampfregeln fÃ¼hren
zur Verbindungsablehnung. Der rein optische Schalter `EnableSpecialVisual` und
Tastenbelegungen dÃ¼rfen unterschiedlich sein; den XP-Faktor liefert der Host.

Bestehende gewÃ¶hnliche AusrÃ¼stung bleibt neutral, auch beim Aufwerten.
Neu hergestellte unterstÃ¼tzte AusrÃ¼stung und neue geeignete NPC-Gear-Drops
erhalten eine Itemization-IdentitÃ¤t.
Beim Aufwerten eines bereits identifizierten Gegenstands bleibt dessen gespeicherte
QualitÃ¤t erhalten. `EnableNpcGearDrops` benÃ¶tigt den zentralen Itemization-Schalter
und die Schalter der gewÃ¼nschten AusrÃ¼stungsgruppen. Er ist in frischen Profilen
ausgeschaltet. Bestehende GegenstÃ¤nde und vergangene Tode werden nicht neu
gewÃ¼rfelt; neue Beute behÃ¤lt ihre QualitÃ¤t beim Aufheben, Ãœbertragen und Laden.
Die kuratierte Liste umfasst nicht jede Kreatur. Die Beute folgt der Gegnerart: Trolle kÃ¶nnen etwa TrollausrÃ¼stung und Draugr
EisenausrÃ¼stung hinterlassen. Diese zusÃ¤tzliche Beute ist selten: Die aktuelle
Grundchance liegt je nach Stufe und Sternen bei 1,5 bis 6,05 %. Der getrennte
Affixwurf erfolgt erst, wenn tatsÃ¤chlich ein AusrÃ¼stungsdrop entsteht.
ZusÃ¤tzliche Special-Tasten sind zunÃ¤chst unbelegt;
optional `ArmKey` oder `QuickUseModifier` konfigurieren. Der Modifier verwendet
den normalen PrimÃ¤rangriff. Vorher mÃ¶gliche Tastenkonflikte prÃ¼fen.

### Charaktersicherung und Wiederherstellung

Mastery legt nach einem gesunden Charakterspeichervorgang automatisch eine lokale
Sicherung an. Erfasst werden der Fortschritt aller 21 Mastery-Skills und ihre
Charakterfreischaltungen sowie tatsÃ¤chlich im Charakterinventar gehaltene
Mastery-GegenstÃ¤nde und AusrÃ¼stung mit Mastery-QualitÃ¤t. QualitÃ¤t und gespeicherte
Eigenschaften bleiben erhalten. AusgerÃ¼stete Items und Equipment and Quick Slots
3.1.3 einschlieÃŸlich Mastery-KÃ¶cher werden unterstÃ¼tzt. Welttruhen, GrÃ¤ber und
separate Tascheninventare sind nicht enthalten.

Fehlt beim nÃ¤chsten gesunden Laden etwas oder ist der gespeicherte Fortschritt
niedriger, erscheint eine Vorschau, bevor die alte Sicherung ersetzt wird.
Ãœber **Mastery-Sicherung** im Inventar kannst du sie erneut Ã¶ffnen. PrÃ¼fe die
angezeigten Fertigkeiten und GegenstÃ¤nde und wÃ¤hle:

- **Wiederherstellung prÃ¼fen** und **Verlust bestÃ¤tigen und wiederherstellen**, um
  die angezeigten Werte zurÃ¼ckzuholen. Zuerst freie normale InventarplÃ¤tze schaffen;
  zurÃ¼ckgeholte GegenstÃ¤nde werden nicht automatisch ausgerÃ¼stet.
- **Aktuellen Stand behalten**, um den gegenwÃ¤rtigen Charakterstand zu Ã¼bernehmen.
- **SpÃ¤ter / schlieÃŸen**, um die bisherige Sicherung fÃ¼r eine spÃ¤tere Entscheidung
  zu erhalten.

Es erfolgt keine automatische Wiederherstellung. Ohne laufende Mastery-Mod kann
die Sicherung Weitergabe, Verbrauch und Tod nicht beobachten. Fehlende Items
kÃ¶nnen noch in einer Truhe, einem Grab oder bei einem Mitspieler liegen; eine
bestÃ¤tigte Wiederherstellung kÃ¶nnte sie verdoppeln. Die erste Sicherung kann
frÃ¼here Verluste nicht rekonstruieren. Verbrauchte Ressourcen, eingelÃ¶ste
Belohnungen und weltseitige Slayer-Konten werden nicht zurÃ¼ckgesetzt.
Eine unterbrochene bestÃ¤tigte Wiederherstellung bleibt zur manuellen PrÃ¼fung
gesperrt. Ihre Dateien behalten und nicht lÃ¶schen, um eine erneute Ausgabe
zu erzwingen.

**Sicherungsordner anzeigen** im Fenster zeigt den Ablageort. Die Dateien liegen
unter `MasteryRecovery` im aktiven Valheim-Saveverzeichnis und werden **nicht
automatisch Ã¼ber Steam Cloud synchronisiert**. Beim GerÃ¤tewechsel den gesamten
Recovery-Ordner zusammen mit den Charaktersaves kopieren. Ein Wechsel zwischen
lokalem und Cloud-Speicher erfordert eine PrÃ¼fung. VollstÃ¤ndige Charakter- und
Weltsicherungen weiterhin separat anlegen.

### Steuerung

| Taste | Aktion |
| --- | --- |
| F1 | Kampfstil wechseln |
| Q | AusgewÃ¤hlte Ortung aktivieren |
| F2 | Ortungsmodus wechseln |
| Umschalt + F2 | Native Verbindungsinformationen |
| F3 | Freigeschalteten Runebound-Zauber wechseln |
| R halten | HUD-Cursor fÃ¼r Kampfstil, Ortung und Gebet; â€žWaffe wegsteckenâ€œ vorher auf T legen |
| R halten und SP anklicken | Dyrnwyn-Special vorbereiten oder abbrechen; danach normal angreifen |
| Controller-Ansichtstaste + Schultertasten | Rechtes HUD durchgehen; untere Aktionstaste bestÃ¤tigt |
| Controller-Ansichtstaste + Steuerkreuz hoch/runter | Gebetsliste durchgehen; rechte Aktionstaste schaltet Gebet |
| Linke GEBET-Lasche berÃ¼hren | Gebetsliste Ã¶ffnen oder schlieÃŸen |
| Mittlere Maustaste halten | Bogen-/Armbrustzoom |
| Strg + F1 | Berserk des Slayer Mastery Cape |
| Umschalt + F1 | KontextabhÃ¤ngige Bergbau-, HolzfÃ¤ll- oder Segelkraft |
| Alt + F1 | KontextabhÃ¤ngige Jagd-, Baukunst- oder Angelkraft |
| Alt + Q | Slayer-Jagdinstinkt, sobald freigeschaltet |

Die Tasten sind konfigurierbar. Das Apex Mastery Cape verwendet dieselben
kontextabhÃ¤ngigen Tasten. Q aktiviert nur die gewÃ¤hlte Ortung. Die Mod entfernt
die Auto-Run-Belegung. SP unterstÃ¼tzt auch Touch und Controllerfokus; die
Buttonbezeichnungen kÃ¶nnen je nach Controllerlayout abweichen.

### Koop, Sicherungen und Updates

Slayer-Koop am Brett zu zweit beginnen; der Partner muss vor dem ersten Kill
beitreten. Berechtigte Teilnehmer in der NÃ¤he erhalten dieselben Slayer-Kill-XP.
FÃ¼r die gemeinsamen Abschlussmarken mÃ¼ssen beide beim letzten Kill leben und
hÃ¶chstens 70 m vom Ziel entfernt sein. Multiplayer bleibt Beta, insbesondere
Wiederverbindungen, Besitzerwechsel und lange Sitzungen. Dedizierte Server sind
experimentell.

ZusÃ¤tzlich zu Charakteren und Welten den Ordner
`BepInEx/config/ValheimMastery/` sichern. Er enthÃ¤lt die Slayer-Datei
`slayer-<world-id>.json` und das Kampf-XP-Journal `combat-coop-<world-id>.tsv` des
Hosts. Ein DLL-Update setzt diese Dateien nicht zurÃ¼ck. Vor einer mÃ¶glichen
Wiederherstellung eines unterbrochenen Journalschreibvorgangs wird eine
`.recovery-*.bak`-Kopie angelegt. BeschÃ¤digte abgeschlossene EintrÃ¤ge oder ein
nicht eindeutig lesbares altes Dateiende stoppen die gemeinsamen Kampf-XP;
der Fehler steht im Log. Das Journal nicht zum Erzwingen eines Resets lÃ¶schen.
Ã„ltere Mastery-Versionen kÃ¶nnen neue JournaleintrÃ¤ge mit PrÃ¼fsumme nicht lesen.
Den Ordner deshalb vor dem Update sichern. FÃ¼r einen VersionsrÃ¼ckgang genÃ¼gt
der DLL-Tausch allein nicht; dazu eine passende Journalsicherung wiederherstellen.

Valheim vor Updates schlieÃŸen. Scheitert Masterys Initialisierung, wird der Start
deaktiviert und eigene Patches und Komponenten werden aufgerÃ¤umt. Ursache in
`BepInEx/LogOutput.log` prÃ¼fen, beheben und das Spiel neu starten.

Die ersetzten Smoothbrain-Mods Mining, Lumberjacking, Blacksmithing, Farming,
Foraging, Cooking und Sailing nicht gleichzeitig verwenden. Erst sichern,
dann diese Plugins deaktivieren; unterstÃ¼tzter alter Fortschritt kann ohne ihre
DLLs Ã¼bernommen werden. Andere Kampfumbauten, BetterArchery, weitere Skill-
Ersatzmods und SkillBonusTooltips gehÃ¶ren nicht zur unterstÃ¼tzten Ausgangsbasis.

Mastery speichert Fortschritt, GegenstÃ¤nde und Weltobjekte. Einen bestehenden
Charakter deshalb nicht zur Probe ohne Mods laden. FÃ¼r eine saubere RÃ¼ckkehr
zum Zustand vor Mastery eine entsprechende Sicherung wiederherstellen.

### Lokale Daten und bekannte Grenzen

Anonyme Balancingdaten werden ausschlieÃŸlich lokal unter
`BepInEx/ValheimMastery/balancing` gespeichert: XP-Quellen, AktivitÃ¤tsfenster,
ErtrÃ¤ge, Boni und Ressourcen-/Kampfwerte. Es werden weder Daten Ã¼bertragen
noch Spieler-/Weltnamen, Chat, Netzwerk-IDs oder Koordinaten erfasst.
Mit `EnableBalanceTelemetry = false` unter `[Diagnostics]` kÃ¼nftige Aufzeichnung
abschalten.

- Dorf-BauplÃ¤ne und deren GelÃ¤ndevorbereitung bleiben deaktiviert.
- KÃ¶der locken nur Wildschweine und Hasen. Landende VÃ¶gel kÃ¶nnen Fallen auslÃ¶sen,
  werden aber nicht angelockt.
- Andere Sprachen verwenden Englisch. Das Zehn-Stunden-Ziel benÃ¶tigt Spielpraxis.
- Controllerlayouts kÃ¶nnen Anpassungen benÃ¶tigen; vollstÃ¤ndige Controller-
  UnterstÃ¼tzung und alle Gebetskombinationen sind noch in Entwicklung.
- Weitere Gegner- und Inhaltsmods kÃ¶nnen eigene KompatibilitÃ¤tsanpassungen benÃ¶tigen.
- Auf null reduzierter Schaden entfernt keine bereits aktiven Statuseffekte.

Fehler und Balancing bitte Ã¼ber die oben verlinkten GitHub Issues melden.
Versionen, XP-Faktor, Mods, Host-/Clientrolle, genaue Schritte sowie erwartetes
und tatsÃ¤chliches Ergebnis angeben. FÃ¼r Balancing auch Stufe, TÃ¤tigkeit und
ungefÃ¤hre Dauer nennen. Nur den relevanten Ausschnitt aus `BepInEx/LogOutput.log`
anhÃ¤ngen; persÃ¶nliche Pfade und private Serverdetails entfernen. Ã–ffentliche
Meldungen sind fÃ¼r andere Nutzer sichtbar. Eine Vorlage steht in `FEEDBACK.md`.

Asset- und KompatibilitÃ¤tsangaben stehen in `NOTICE.md`.
