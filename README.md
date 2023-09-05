# LOONY-TECH-API

# Anleitung: LOONY-TECH API mit Nightbot verwenden

**Deutsche Anleitung: LOONY-TECH API mit Nightbot verwenden**

Möchtest du die LOONY-TECH API für deinen Nightbot nutzen? Kein Problem! Hier ist, wie du es machen kannst:

**Schritt 1: Nightbot-Befehle erstellen**

1. Melde dich bei deinem Nightbot-Dashboard an: [https://nightbot.tv/dashboard](https://nightbot.tv/dashboard).

2. Klicke auf die Registerkarte "Commands" (Befehle), um benutzerdefinierte Befehle zu erstellen.

3. **Lurk-Befehl**:
   - Befehlsname: `lurk`
   - Nachricht: `!lurk $(user) $(channel) [DEINE_API-URL]/nightbot/lurk?user=$(user)&channel=$(channel)`
   - Userlevel: Everyone (Jeder)

4. **Reset-Lurk-Befehl**:
   - Befehlsname: `resetlurk`
   - Nachricht: `!resetlurk $(channel) [DEINE_API-URL]/nightbot/reset_lurk?channel=$(channel)`
   - Userlevel: Moderator (Moderator)

5. **Back-Befehl**:
   - Befehlsname: `back`
   - Nachricht: `!back $(user) $(channel) [DEINE_API-URL]/nightbot/back?user=$(user)&channel=$(channel)`
   - Userlevel: Everyone (Jeder)

6. **Randomnumber-Befehl**:
   - Befehlsname: `randomnumber`
   - Nachricht: `!randomnumber $(querystring) [DEINE_API-URL]/nightbot/random/number?min=$(1)&max=$(2)`
   - Userlevel: Everyone (Jeder)

7. **Twitchfollowage-Befehl**:
   - Befehlsname: `twitchfollowage`
   - Nachricht: `!twitchfollowage $(querystring) [DEINE_API-URL]/twitch/followage?user=$(1)&channel=$(2)`
   - Userlevel: Everyone (Jeder)

**Hinweis**: Ersetze `[DEINE_API-URL]` durch die URL deiner eigenen API.

**Schritt 2: Befehle verwenden**

Jetzt kannst du die LOONY-TECH API in deinen Nightbot-Befehlen verwenden, um benutzerdefinierte Aktionen für deinen Twitch-Kanal auszuführen.

### Beispielverwendung:
- `!lurk` - Startet den Lurk-Modus für den aktuellen Benutzer im aktuellen Kanal.
- `!resetlurk` - Setzt die Lurk-Daten für den aktuellen Kanal zurück (nur für Moderatoren verfügbar).
- `!back` - Zeigt an, wie lange der Benutzer im Lurk-Modus war.
- `!randomnumber 1 100` - Generiert eine zufällige Zahl zwischen 1 und 100.
- `!twitchfollowage Benutzername Kanalname` - Zeigt an, wie lange ein Benutzer einem Kanal folgt.

Denke daran, deine Twitch-Bot-Autorisierungstoken sicher zu speichern und niemals öffentlich zu veröffentlichen. Implementiere außerdem Sicherheitsmaßnahmen, um deinen Twitch-Bot und den API-Zugriff zu schützen.

**English Guide: Using LOONY-TECH API with Nightbot**

Would you like to use the LOONY-TECH API with your Nightbot? No problem! Here's how you can do it:

**Step 1: Create Nightbot Commands**

1. Log in to your Nightbot dashboard: [https://nightbot.tv/dashboard](https://nightbot.tv/dashboard).

2. Click on the "Commands" tab to create custom commands.

3. **Lurk Command**:
   - Command Name: `lurk`
   - Message: `!lurk $(user) $(channel) [YOUR_API_URL]/nightbot/lurk?user=$(user)&channel=$(channel)`
   - Userlevel: Everyone

4. **Reset Lurk Command**:
   - Command Name: `resetlurk`
   - Message: `!resetlurk $(channel) [YOUR_API_URL]/nightbot/reset_lurk?channel=$(channel)`
   - Userlevel: Moderator

5. **Back Command**:
   - Command Name: `back`
   - Message: `!back $(user) $(channel) [YOUR_API_URL]/nightbot/back?user=$(user)&channel=$(channel)`
   - Userlevel: Everyone

6. **Random Number Command**:
   - Command Name: `randomnumber`
   - Message: `!randomnumber $(querystring) [YOUR_API_URL]/nightbot/random/number?min=$(1)&max=$(2)`
   - Userlevel: Everyone

7. **Twitch Followage Command**:
   - Command Name: `twitchfollowage`
   - Message: `!twitchfollowage $(querystring) [YOUR_API_URL]/twitch/followage?user=$(1)&channel=$(2)`
   - Userlevel: Everyone
  
**Step 2: Using Commands**

Now you can use the LOONY-TECH API in your Nightbot commands to perform custom actions for your Twitch channel.

### Example Usage:
!lurk - Initiates lurk mode for the current user in the current channel.
!resetlurk - Resets lurk data for the current channel (only available to moderators).
!back - Indicates how long the user has been in lurk mode.
!randomnumber 1 100 - Generates a random number between 1 and 100.
!twitchfollowage Username ChannelName - Indicates how long a user has been following a channel.
