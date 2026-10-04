## 0.17.2 — 04 October 2026

- The Construction board defines one shared circular building area. Actual workbenches, forges, stonecutters and other building stations inside it supply their building permission throughout that area. Stations are still required.
- With AzuCraftyBoxes installed and enabled, accessible chests in the same area supply its normal crafting/building actions. Distant chests use lightweight network representations without loading the entire surrounding terrain. Existing payment and access rules remain in effect.
- Construction milestones at 10/30/50/70/90 unlock another 25 metres of area radius each; wearing the Construction cape unlocks another 100 metres. Set the radius at the board: 20 metres initially, up to 245 metres. A saved area upgrade remains when the contributor leaves or removes the cape. These bonuses no longer extend personal placement distance.
- Existing rectangular areas retain a minimum radius covering their corners. Without a board, native station ranges and the configured chest range apply.
- Construction boards display the existing Construction skill icon. German/English descriptions explain the new radius.
- Production totals are indexed instead of rescanning the transaction history for each claim. Repeated identical minimap saves reuse a bounded compression result; native save bytes remain unchanged. No blanket FPS improvement is claimed.
- Corrected German Agility/Woodcutting labels and leaderboard tabs. Existing character progress and configuration remain intact. Update clients and server together.

Deutsch: Das Baumeisterbrett legt ein gemeinsames Baugebiet fest. Vorhandene Stationen und zugängliche Kisten darin gelten für den gesamten Kreis. Die Baukunst-Boni erweitern diesen Kreis statt der persönlichen Platzierungsdistanz. Den Radius am Brett einstellen; gespeicherte Erweiterungen bleiben bestehen. Alte Rechtecke bleiben vollständig abgedeckt. Ohne Brett gelten die bisherigen Stations- und Kistenreichweiten. Das Brett zeigt das Baukunst-Symbol.

Windows installer V72 retains the optional local diagnostics. Reports stay in Downloads/mastery_diag.zip; no automatic upload. Test-only cape colour concepts are excluded.

## 0.17.1 — 04 October 2026

- Production XP journals now append small durable transactions instead of rewriting the complete history for every output. Existing progress is retained. Back up the entire Mastery configuration directory, including `.tsv` and `.tsv.wal` files, while the server is stopped. Do not downgrade by replacing only the DLL after new production has been recorded.
- Character recovery avoids redundant saves immediately after a successful save and unnecessary temporary copies during packet verification. Recovery protections remain enabled; no measured FPS improvement is claimed.
- Leaderboard responses are bounded during download. The board has a visible scrollbar, direct skill selection and localized numbers.
- Slayer reward details now match the award formulas. Magic and Prayer unlocks are included in the general milestone list; staff tooltips reflect configured keys.
- High Alchemy adds controller focus, navigation and separate confirmation. A physical controller gameplay check remains outstanding.
- The leaderboard remains voluntary, self-reported Community progression. Server-verified competition is not enabled in this version.

Deutsch: Produktionsjournale speichern einzelne Änderungen statt jedes Mal die gesamte Historie. Rangliste mit sichtbarer Scrollleiste und direkter Skillwahl, korrigierte Slayer-Angaben, vollständige Magie-/Gebetsfreischaltungen und konfigurierte Stabtasten. Hohe Alchemie erhält Controllerführung mit getrennter Bestätigung. Bestehende XP und Einstellungen bleiben erhalten. Clients und Server gemeinsam aktualisieren. Die Rangliste bleibt ungeprüfte Community-Wertung.

**Windows installer V71:** includes the corrected local process-memory diagnostics.

## Core 0.17.0 / Installer V70 — 04 October 2026

- Online leaderboard: open Skills → Leaderboard. Top 100 overall/per skill, player details and your own rank. Joining is voluntary: the Join button publishes your character name and 21 skill XP values. Changes upload at most every three minutes. Access codes support recovery; keep them private. Leave/delete removes your public profile. Values are self-reported and unverified; Standard and Test/multiplier lists are separate.
- Levels still cap at 100 (1,439,116 XP). Each skill can now accumulate up to 200 million XP; maximum total level 2,100 and total XP 4.2 billion. Previously discarded excess XP is not reconstructed.
- Smithing capacity milestones now include charcoal kilns: +20/40/60/80/100% wood capacity at levels 20/40/60/80/100. No automatic filling or change to output.
- Fix: full-health tamed animals with an omitted health save field are no longer treated as dead by portal travel. Existing ownership, following, range and safe landing restrictions remain. A complete multiplayer animal-portal test is still outstanding.

Deutsch: Fertigkeiten → Leaderboard öffnet die globale Rangliste. Erst „Teilnehmen“ veröffentlicht Name und 21 Skillwerte; kein automatischer Beitritt. Zugangscode privat sichern, Profil bei Bedarf löschen. Die Werte sind selbst gemeldet und ungeprüft. Keine Steam-ID, Hardwaredaten, Spielstände oder Diagnosearchive werden dafür übertragen. Cloudflare verarbeitet technische Verbindungsdaten; die Anwendung speichert keine IP-Adressen.

Client und Server gemeinsam aktualisieren. Vorhandene Spielstände, XP und Einstellungen bleiben erhalten. Neue Profile starten mit XP ×1. Der lokale Diagnosebericht bleibt lokal. Keine privaten Bossmodule oder persönlichen Zustellhelfer enthalten.

## Core 0.16.53 / Installer V67 — 03 October 2026

- Tamed animals within five metres of the portal can accompany a completed player portal trip when their network object is confirmed to be locally owned. Wolves must be following that exact player. The same animal/ZDO is moved; animals are not cloned or replaced.
- Travel requires a loaded destination and a safe free landing position. Dead/wild animals, ridden or attached animals and animals behind a closed wall are excluded. Cancelled trips move nothing. Remote-owned animals or ownership changes leave animals at the origin; remote-owner transport is not guaranteed.
- Reduces repeated allocations in Prayer updates and cape inventory checks. XP HUD text is refreshed when its displayed state changes. No measured FPS gain is claimed.

Deutsch: Gezähmte Tiere im Umkreis von fünf Metern um das betretene Portal können nach abgeschlossener Reise folgen, sofern ihr Netzwerkobjekt weiterhin bestätigt lokal verwaltet wird. Wölfe müssen genau dem reisenden Spieler folgen. Derselbe Tier-ZDO bleibt erhalten; keine Kopien. Das Ziel muss geladen sein und einen sicheren freien Landeplatz bieten. Fremdverwaltete Tiere und Tiere mit Besitzwechsel bleiben zurück. Abgebrochene Reisen verschieben nichts. Reduzierte wiederholte Speicherallokationen bei Gebet/Cape-Prüfungen und bedarfsgerechte XP-HUD-Texte; kein versprochener oder bereits gemessener FPS-Gewinn.

Targeted native/policy checks, independent reviews and the release build passed. Actual portal gameplay, sector-unload ownership transitions and multiplayer travel remain unverified in game. This is deliberately conservative local-owner support, not a complete remote-owner transport protocol.

Installer V67 retains the same comfort mods and MasteryDiagnostics 1.0.0 as V66. No local hotpath probe, personal item helper, private encounter module or terrain experiment is included. Existing progress/settings remain; new profiles use XP x1. Update clients and server together.

## Core 0.16.52 / Installer V66 — 03 October 2026

- Combat-style tooltips omit zero-valued bonuses.
- Skillcape cooldowns use the native status bar and their matching icons.
- The Prayer bar shows continuous remaining points and updates immediately.
- Both Prayer drink icons use the native round corked bottle with cyan liquid, preserving the original cork, shading and transparency.
- Prayer Potion restores 60 points; Prayer Mead remains at 20. Recipes and drinking cooldowns are unchanged.

Deutsch: Kampfhaltungen zeigen keine wirkungslosen Nullboni mehr. Skillcape-Abklingzeiten erscheinen mit passenden Symbolen in der nativen Statusleiste. Der Gebetsbalken zeigt den verbleibenden Vorrat stufenlos und aktualisiert sofort. Beide Gebetsgetränke erhalten native runde Flaschenicons mit cyanfarbenem Inhalt; Korken, Schattierung und Transparenz bleiben erhalten. Der Gebetstrank stellt 60 Punkte wieder her, Gebetsmet weiterhin 20; Rezepte und Trinkpausen bleiben gleich.

Installer V66 retains the same comfort mods and MasteryDiagnostics 1.0.0 as V65. No personal delivery helpers, private encounter modules or terrain experiments are included. Existing progress and settings remain; fresh profiles use XP x1. Update Core on clients and server together.

Targeted regression checks, independent code review and the release build passed. No new background game was launched for this release.

## 0.16.51 / Installer V65 — 03 October 2026

- Mining XP now covers the native small-stone, tin and obsidian drop paths, including legitimate zero-weight stone drops; awards remain based on actual resources.
- Redesigned magic staves and prestige Slayer helmets; inherited staff effects removed. The Prayer HUD icon below its bar now scales with the bar width.
- Mastery and Max capes hang on native wall stands with a rolled cloth edge, without the worn collar or clasps. All eight Max Cape styles remain available.
- Construction 100 recovers paid initial recipe ingredients previously excluded from manual demolition refunds. Free saved materials, later-added fuel and consumed feast portions are not duplicated; ordinary native refunds and XP remain unchanged.
- Combat level uses Attack, Strength, Defence, Hitpoints and Prayer, capped at 126. Equipment, Ranged and Magic are excluded; progress is not reset. Native skill title and optional BetterUI display agree.
- Installer V65 retains the optional client-side local diagnostics from V64. No private modules or personal item-delivery helpers are included.

Deutsch: Bergbau-XP fuer Stein/Zinn/Obsidian korrigiert; neue Stab- und Prestigehelmgestaltung sowie ein mit der Balkenbreite skaliertes Gebets-HUD-Symbol unter dem Balken. Wandcapes ohne Kragen, mit eingerolltem Stoffrand und acht Max-Cape-Stilen. Baukunst 100 erstattet bezahlte Anfangszutaten beim manuellen Abriss, ohne kostenlose Materialien oder nachgefuellten Brennstoff zu vermehren. Kampfstufe aus Angriff, Staerke, Verteidigung, Lebenspunkten und Gebet bis 126; vorhandene XP bleiben erhalten. Clients und Server gemeinsam aktualisieren. Bestehende Einstellungen bleiben, neue Profile starten mit XP x1.

Validation: targeted source/native contracts, release build and independent review passed. Visual feedback was incorporated during test play; this is not a claim that every multiplayer edge case has been reproduced.

# Valheim Mastery Installer

Hier gibt es das vollständige Windows-Installationspaket für Valheim Mastery. Es enthält die Mod, BepInEx, die benötigten Abhängigkeiten und abgestimmte Komfortmods.

**[Aktuellen Installer herunterladen](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/releases/latest/download/Valheim-Mastery-Installer.zip)**

Aktuell: **Valheim Mastery 0.16.53 / Installer V67**. Angriffe lassen sich mit Blocken/Ausweichen unterbrechen, einschließlich Fernkampf und Magie. Bereits bezahlte Ressourcen bleiben verbraucht. Build-/Vertragschecks bestanden; praktische Animations- und Multiplayer-Abnahme offen. Stations-XP und Slayer verwenden gespeicherte Host-/Welt-Belege; Stationsproduktion ordnet entfernte Spieler anhand ihrer Netzwerk-Charakterdaten zu. Gebetsopfer werden nach erfolgreicher Transaktion protokolliert; verdorrte Knochen sind als Opfer zugelassen. Rewards 2.0, Cape-Aktionen, Herstellungsfolgen, verbesserte Steuerungsbeschreibung und native Buff-Anzeige sind enthalten. Cape-Namen werden zwischengespeichert, ohne die Inventarprüfungen zu umgehen.

**Weiter enthalten seit V64: lokale Leistungsdiagnose.** Sie startet mit Valheim und aktualisiert alle **15 Minuten** dieselbe Datei **`Downloads/mastery_diag.zip`** mit den bisherigen Messdaten der Sitzung. Kein automatischer Upload. Enthalten sind FPS/Bildzeiten, CPU-/Speichermesswerte, verfügbare GPU-Messwerte, Software-/Hardwareversionen und ausgewählte Grafikeinstellungen. Keine Rohlogs, IP-/Serveradressen, Konten-/Spieler-/Weltnamen, Passwörter oder persönlichen Pfade. Fehler werden nur gezählt. Nicht verfügbare Messwerte sind gekennzeichnet. Beim Beenden wird ein letzter Speicherlauf versucht; bei Absturz oder blockierter Datei bleibt gegebenenfalls nur der letzte Checkpoint. Eine neue Sitzung ersetzt den vorherigen Bericht beim ersten Speichern; zum Aufheben vorher kopieren. Abschalten: `Enabled = false` unter `[Diagnostics]` in `BepInEx/config/org.valheim.mastery.diagnostics.cfg`, anschließend Valheim neu starten. Der Diagnose-Recorder bleibt unverändert; Core 0.16.53 auf Clients und Server gemeinsam aktualisieren.

**English:** Automatic local diagnostics remain included: the same `Downloads/mastery_diag.zip` is updated every 15 minutes for the current session, with a best-effort final save on exit. No automatic upload or raw logs; no IP/server addresses, account/player/world names, passwords or personal paths. Unsupported metrics are marked unavailable. A new session replaces the previous report at its first checkpoint. Disable `Enabled` in the diagnostics config and restart. Update Core 0.16.53 on clients and server together.

**English:** Station and Slayer credits now use persistent host/world receipts; station credit resolves remote players through network character records. Prayer offerings are logged after successful completion and withered bones are accepted. Rewards 2.0, cape actions, production queues, updated control instructions and native status icons are included. Cached cape names reduce temporary allocations while preserving inventory checks.

**Gemeinsam aktualisieren / Update together:** Alle Clients und der Server benötigen Version 0.16.53 für das neue Host-Kampf-XP-Protokoll. Getrennte Hostinstallationen derselben Welt verwenden unabhängige Checkpoints. Vorhandene XP bleiben erhalten; historische fehlende Gutschriften werden nicht automatisch nachgetragen. All clients and the server must update for the new host-scoped combat-credit protocol. Existing earned XP remains; old unapplied credits are not automatically restored.

**Prüfgrenzen / Validation:** The full build and focused station/Slayer checks passed; native multiplayer acceptance of the new credit protocol is outstanding. The earlier remote-owner combo/refund proof remains open. Quellenprüfungen und Gesamtbuild bestanden; native Abnahme des neuen Protokolls und Remote-Kombo-Nachweis stehen aus. These are validation gaps, not confirmed product defects.

Standard progression uses **XP x1**. Existing individual multipliers are retained. Standardfortschritt ist **XP x1**; vorhandene individuelle Einstellungen bleiben erhalten.

Back up `BepInEx/ValheimMastery/combat-host-identity-v2.txt` with the host journals and world. Do not delete it as an XP reset. Hostidentität mit Journalen und Welt sichern, nicht als XP-Reset löschen.

Neu sind automatische lokale Sicherungen für die 21 Mastery-Skillfortschritte und gehaltene Mastery-Gegenstände. **Mastery-Sicherung** im Inventar öffnet die Vorschau: echten Verlust ausdrücklich bestätigen, aktuellen Stand behalten oder später entscheiden. Truhen und Gräber werden nicht gesichert; Weitergaben ohne laufende Mod bleiben unbekannt. Unterbrochene Wiederherstellungen bleiben zur manuellen Prüfung gesperrt. Über **Sicherungsordner anzeigen** lassen sich die Dateien finden. Beim Gerätewechsel mitnehmen: keine automatische Steam-Cloud-Synchronisierung.

**English:** Automatic local backups cover all 21 Mastery skill progressions and held Mastery items. Open **Mastery recovery** from the inventory to review and explicitly confirm genuine loss, keep current state or decide later. Chests and graves are excluded; transfers while the mod is absent are unknown. Interrupted recoveries stay blocked for review. Use **Show backup folder** and copy those files when changing devices; Steam Cloud does not transfer them automatically.

Valheim auf allen Rechnern vollständig beenden, die ZIP entpacken und `Installieren.exe` starten. Der Installer sichert ersetzte Dateien und erhält Spielstände, vorhandene XP-Werte und persönliche Einstellungen. Acht Itemization-Schalter einschließlich Gegnerdrops sowie zwei Special-Schalter werden gezielt aktiviert, insgesamt zehn. Neue Installer-Profile verwenden XP ×1. Vorhandene individuelle XP-Multiplikatoren bleiben erhalten. Alle Mitspieler benötigen dieselbe Paketversion und dieselben Spielregeln. Die SHA-256-Prüfsumme steht im jeweiligen Release.

Das Paket ist für Windows 10/11 x64 und die im Release genannte Steam-Valheim-Version gebaut. Es ist ein inoffizielles Fanprojekt, inspiriert von RuneScape/OSRS, ohne Verbindung zu Iron Gate oder Jagex. Drittanbieter-Mods bleiben Eigentum ihrer jeweiligen Autoren; ihre Hinweise und Lizenzen liegen im Paket.

Ältere Versionen bleiben unter [Releases](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/releases) verfügbar. Bei einem Update dieselbe Installationsanleitung befolgen. Der Link oben zeigt immer auf den neuesten Release.

Fehler oder Balancing-Probleme bitte über [GitHub Issues](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/issues/new/choose) melden. Der Bericht ist öffentlich; private Serverdaten und persönliche Pfade aus Logs entfernen.
