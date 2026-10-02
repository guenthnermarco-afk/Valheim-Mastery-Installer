# Valheim Mastery Installer

Hier gibt es das vollständige Windows-Installationspaket für Valheim Mastery. Es enthält die Mod, BepInEx, die benötigten Abhängigkeiten und abgestimmte Komfortmods.

**[Aktuellen Installer herunterladen](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/releases/latest/download/Valheim-Mastery-Installer.zip)**

Aktuell: **Valheim Mastery 0.16.48 / Installer V61**. Rewards 2.0, Cape-Aktionen, Herstellungsfolgen, verbesserte Steuerungsbeschreibung und native Buff-Anzeige sind enthalten. Cape-Namen werden zwischengespeichert, ohne die Inventarprüfungen zu umgehen.

**English:** Rewards 2.0, cape actions, production queues, updated control instructions and native status icons are included. Cached cape names reduce temporary allocations while preserving inventory checks.

**Gemeinsam aktualisieren / Update together:** Alle Clients und der Server benötigen Version 0.16.48 für das neue Host-Kampf-XP-Protokoll. Getrennte Hostinstallationen derselben Welt verwenden unabhängige Checkpoints. Vorhandene XP bleiben erhalten; historische fehlende Gutschriften werden nicht automatisch nachgetragen. All clients and the server must update for the new host-scoped combat-credit protocol. Existing earned XP remains; old unapplied credits are not automatically restored.

**Prüfgrenzen / Validation:** 39 focused source checks and the full build passed; native multiplayer acceptance of the new credit protocol is outstanding. The earlier remote-owner combo/refund proof remains open. Quellenprüfungen und Gesamtbuild bestanden; native Abnahme des neuen Protokolls und Remote-Kombo-Nachweis stehen aus. These are validation gaps, not confirmed product defects.

Standard progression uses **XP x1**. Existing individual multipliers are retained. Standardfortschritt ist **XP x1**; vorhandene individuelle Einstellungen bleiben erhalten.

Back up `BepInEx/ValheimMastery/combat-host-identity-v2.txt` with the host journals and world. Do not delete it as an XP reset. Hostidentität mit Journalen und Welt sichern, nicht als XP-Reset löschen.

Neu sind automatische lokale Sicherungen für die 21 Mastery-Skillfortschritte und gehaltene Mastery-Gegenstände. **Mastery-Sicherung** im Inventar öffnet die Vorschau: echten Verlust ausdrücklich bestätigen, aktuellen Stand behalten oder später entscheiden. Truhen und Gräber werden nicht gesichert; Weitergaben ohne laufende Mod bleiben unbekannt. Unterbrochene Wiederherstellungen bleiben zur manuellen Prüfung gesperrt. Über **Sicherungsordner anzeigen** lassen sich die Dateien finden. Beim Gerätewechsel mitnehmen: keine automatische Steam-Cloud-Synchronisierung.

**English:** Automatic local backups cover all 21 Mastery skill progressions and held Mastery items. Open **Mastery recovery** from the inventory to review and explicitly confirm genuine loss, keep current state or decide later. Chests and graves are excluded; transfers while the mod is absent are unknown. Interrupted recoveries stay blocked for review. Use **Show backup folder** and copy those files when changing devices; Steam Cloud does not transfer them automatically.

Valheim auf allen Rechnern vollständig beenden, die ZIP entpacken und `Installieren.exe` starten. Der Installer sichert ersetzte Dateien und erhält Spielstände, vorhandene XP-Werte und persönliche Einstellungen. Acht Itemization-Schalter einschließlich Gegnerdrops sowie zwei Special-Schalter werden gezielt aktiviert, insgesamt zehn. Neue Installer-Profile verwenden XP ×1. Vorhandene individuelle XP-Multiplikatoren bleiben erhalten. Alle Mitspieler benötigen dieselbe Paketversion und dieselben Spielregeln. Die SHA-256-Prüfsumme steht im jeweiligen Release.

Das Paket ist für Windows 10/11 x64 und die im Release genannte Steam-Valheim-Version gebaut. Es ist ein inoffizielles Fanprojekt, inspiriert von RuneScape/OSRS, ohne Verbindung zu Iron Gate oder Jagex. Drittanbieter-Mods bleiben Eigentum ihrer jeweiligen Autoren; ihre Hinweise und Lizenzen liegen im Paket.

Ältere Versionen bleiben unter [Releases](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/releases) verfügbar. Bei einem Update dieselbe Installationsanleitung befolgen. Der Link oben zeigt immer auf den neuesten Release.

Fehler oder Balancing-Probleme bitte über [GitHub Issues](https://github.com/guenthnermarco-afk/Valheim-Mastery-Installer/issues/new/choose) melden. Der Bericht ist öffentlich; private Serverdaten und persönliche Pfade aus Logs entfernen.
