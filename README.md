🛡️ Advanced Tactical Deployment Hub (A.T.D.H.) v1.0
Willkommen beim A.T.D.H. – dem fortschrittlichsten Deployment-System für FiveM. Dieses Skript bietet eine hochmoderne, taktische Benutzeroberfläche (NUI), die speziell für MilSim-, Police- oder Hardcore-Roleplay-Server entwickelt wurde.
🚀 Features
 * Modernes Taktik-Interface: Einzigartiges Design mit Fokus auf Immersion.
 * Job-Based Access: Beschränke Spawnpunkte auf bestimmte ESX-Jobs (z. B. nur Army, Police oder Medic).
 * Echtzeit-Präsenz: Das System erkennt automatisch, wie viele Spieler sich an einer Basis befinden und zeigt dies im Menü an.
 * Last-Location Memory: Ermöglicht den Wiedereinstieg am letzten bekannten Standort direkt aus der Datenbank.
 * High Performance: Das Skript ist extrem optimiert (0.00ms im Idle) und nutzt effiziente Datenbankabfragen via oxmysql.
 * Easy Customization: Ändere Hintergründe, Farben und Spawns in Sekunden.
🛠️ Anforderungen (Dependencies)
Um dieses Skript zu nutzen, müssen folgende Ressourcen auf deinem Server installiert sein:
 * es_extended (ESX Legacy oder v1.Final)
 * oxmysql
📥 Installation
 * Extrahiere den Ordner army_spawn in dein FiveM resources Verzeichnis.
 * Stelle sicher, dass der Ordnername exakt army_spawn lautet.
 * Füge folgende Zeile in deine server.cfg ein:
   ensure army_spawn

 * Starte deinen Server neu oder nutze refresh und start army_spawn.
⚙️ Konfiguration
Alle Einstellungen findest du in der config.lua. Hier ist ein kurzer Guide:
Spawns hinzufügen oder ändern
Du kannst unbegrenzt viele Punkte hinzufügen. Nutze das folgende Format:
{
    name = "Name der Basis",
    coords = vector3(X, Y, Z),
    heading = 0.0, -- Blickrichtung
    jobs = { "jobname1", "jobname2" } -- Wer darf hier spawnen? (Leer lassen für alle)
},

Hintergrundbild ändern
Öffne die Datei html/index.html. Suche nach der Zeile:
url('DEIN_LINK_HIER')
Dort kannst du einfach den Link zu deinem eigenen Bild (z.B. von Imgur oder Discord) einfügen.
📡 Befehle
 * /armyhub - Öffnet das Deployment-Menü manuell (nur für Testzwecke, kann in der client.lua deaktiviert werden).
📄 Support & Lizenz
Dieses Skript wurde für den Einsatz auf ESX-Servern optimiert. Modifikationen am CSS/HTML sind erlaubt, um das Design an deinen Server anzupassen.
