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

Aktuell: **Valheim Mastery 0.16.51 / Installer V65**. Angriffe lassen sich mit Blocken/Ausweichen unterbrechen, einschließlich Fernkampf und Magie. Bereits bezahlte Ressourcen bleiben verbraucht. Build-/Vertragschecks bestanden; praktische Animations- und Multiplayer-Abnahme offen. Stations-XP und Slayer verwenden gespeicherte Host-/Welt-Belege; Stationsproduktion ordnet entfernte Spieler anhand ihrer Netzwerk-Charakterdaten zu. Gebetsopfer werden nach erfolgreicher Transaktion protokolliert; verdorrte Knochen sind als Opfer zugelassen. Rewards 2.0, Cape-Aktionen, Herstellungsfolgen, verbesserte Steuerungsbeschreibung und native Buff-Anzeige sind enthalten. Cape-Namen werden zwischengespeichert, ohne die Inventarprüfungen zu umgehen.

**Neu im Installer V65: lokale Leistungsdiagnose.** Sie startet mit Valheim und aktualisiert alle **15 Minuten** dieselbe Datei **`Downloads/mastery_diag.zip`** mit den bisherigen Messdaten der Sitzung. Kein automatischer Upload. Enthalten sind FPS/Bildzeiten, CPU-/Speichermesswerte, verfügbare GPU-Messwerte, Software-/Hardwareversionen und ausgewählte Grafikeinstellungen. Keine Rohlogs, IP-/Serveradressen, Konten-/Spieler-/Weltnamen, Passwörter oder persönlichen Pfade. Fehler werden nur gezählt. Nicht verfügbare Messwerte sind gekennzeichnet. Beim Beenden wird ein letzter Speicherlauf versucht; bei Absturz oder blockierter Datei bleibt gegebenenfalls nur der letzte Checkpoint. Eine neue Sitzung ersetzt den vorherigen Bericht beim ersten Speichern; zum Aufheben vorher kopieren. Abschalten: `Enabled = false` unter `[Diagnostics]` in `BepInEx/config/org.valheim.mastery.diagnostics.cfg`, anschließend Valheim neu starten. Der Diagnose-Recorder bleibt unverändert; Core 0.16.51 auf Clients und Server gemeinsam aktualisieren.

**English:** Installer V65 adds automatic local diagnostics: the same `Downloads/mastery_diag.zip` is updated every 15 minutes for the current session, with a best-effort final save on exit. No automatic upload or raw logs; no IP/server addresses, account/player/world names, passwords or personal paths. Unsupported metrics are marked unavailable. A new session replaces the previous report at its first checkpoint. Disable `Enabled` in the diagnostics config and restart. Update Core 0.16.51 on clients and server together.

**English:** Station and Slayer credits now use persistent host/world receipts; station credit resolves remote players through network character records. Prayer offerings are logged after successful completion and withered bones are accepted. Rewards 2.0, cape actions, production queues, updated control instructions and native status icons are included. Cached cape names reduce temporary allocations while preserving inventory checks.

**Gemeinsam aktualisieren / Update together:** Alle Clients und der Server benötigen Version 0.16.51 für das neue Host-Kampf-XP-Protokoll. Getrennte Hostinstallationen derselben Welt verwenden unabhängige Checkpoints. Vorhandene XP bleiben erhalten; historische fehlende Gutschriften werden nicht automatisch nachgetragen. All clients and the server must update for the new host-scoped combat-credit protocol. Existing earned XP remains; old unapplied credits are not automatically restored.

**Prüfgrenzen / Validation:** The full build and focused station/Slayer checks passed; native multiplayer acceptance of the new credit protocol is outstanding. The earlier remote-owner combo/refund proof remains open. Quellenprüfungen und Gesamtbuild bestanden; native Abnahme des neuen Protokolls und Remote-Kombo-Nachweis stehen aus. These are validation gaps, not confirmed product defects.

Standard progression uses **XP x1**. Existing individual multipliers are retained. Standardfortschritt ist **XP x1**; vorhandene individuelle Einstellungen bleiben erhalten.

Back up `BepInEx/ValheimMastery/combat-host-identity-v2.txt` with the host journals and world. Do not delete it as an XP reset. Hostidentität mit Journalen und Welt sichern, nicht als XP-Reset löschen.

Neu sind automatische lokale Sicherungen für die 21 Mastery-Skillfortschritte und gehaltene Mastery-Gegenstände. **Mastery-Sicherung** im Inventar öffnet die Vorschau: echten Verlust ausdrücklich bestätigen, aktuellen Stand behalten oder später entscheiden. Truhen und Gräber werden nicht gesichert; Weitergaben ohne laufende Mod bleiben unbekannt. Unterbrochene Wiederherstellungen bleiben zur manuellen Prüfung gesperrt. Über **Sicherungsordner anzeigen** lassen sich die Dateien finden. Beim Gerätewechsel mitnehmen: keine automatische Steam-Cloud-Synchronisierung.

**English:** Automatic local backups cover all 21 Mastery skill progressions and held Mastery items. Open **Mastery recovery** from the inventory to review and explicitly confirm genuine loss, keep current state or decide later. Chests and graves are excluded; transfers while the mod is absent are unknown. Interrupted recoveries stay blocked for review. Use **Show backup folder** and copy those files when changing devices; Steam Cloud does not transfer them automatically.

Valheim auf allen Rechnern vollständig beenden, die ZIP entpacken und `Installieren.exe` starten. Der Installer sichert ersetzte Dateien und erhält Spielstände, vorhandene XP-Werte und persönliche Einstellungen. Acht Itemization-Schalter einschließlich Gegnerdrops sowie zwei Special-Schalter werden gezielt aktiviert, insgesamt zehn. Neue Installer-Profile verwenden XP ×1. Vorhandene individuelle XP-Multiplikatoren bleiben erhalten. Alle Mitspieler benötigen dieselbe Paketversion und dieselben Spielregeln. Die SHA-256-Prüfsumme steht im jeweiligen Release.

Das Paket ist für Windows 10/11 x64 und die im Release genannte Steam-Valheim-Version gebaut. Es ist ein inoffizielles Fanprojekt, inspiriert von RuneScape/OSRS, ohne Verbindung zu Iron Gate oder Jagex. Drittanbieter-Mods bleiben Eigentum ihrer jeweiligen Autoren; ihre Hinweise und Lizenzen liegen im Paket.

Ältere Versionen bleiben unter [Releases](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/releases) verfügbar. Bei einem Update dieselbe Installationsanleitung befolgen. Der Link oben zeigt immer auf den neuesten Release.

Fehler oder Balancing-Probleme bitte über [GitHub Issues](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/issues/new/choose) melden. Der Bericht ist öffentlich; private Serverdaten und persönliche Pfade aus Logs entfernen.
