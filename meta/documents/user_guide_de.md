# plentyDrive vorgestellt

Durch das neue plentymarkets Tool plentyDrive werden zeitraubende Plugin-Bereitstellungen durch die Synchronisierung einer lokalen Inbox mit dem Stage-Modus des plentymarkets Systems verkürzt.

## plentyDrive installieren

Laden Sie plentyDrive für Ihr Betriebssystem herunter und folgen Sie den Installationsanweisungen.

## plentyDrive einrichten

Richten Sie plentyDrive wie nachfolgend beschrieben ein.

1. Öffnen Sie plentyDrive.
2. Geben Sie Ihre plentymarkets Domain ein. Benutzen Sie dafür https:// bzw. http://.
3. Geben Sie Ihre Login-Daten ein.
4. Klicken Sie auf **Login**.<br />→ plentyDrive wird mit Ihrem plentymarkets System verbunden.
5. Klicken Sie auf **Einstellungen**.
6. Wählen Sie einen lokalen Ordner for die Synchronisierung mit der Plugin-Inbox Ihres plentymarkets Systems.
7. **Speichern** Sie die Einstellungen.<br />→ plentyDrive wird neugestartet.<br />→ Die Einrichtung ist abgeschlossen.

## plentyDrive verwenden

plentyDrive kann die Wartezeit beim Bearbeiten von Plugins stark verkürzen. In diesem Kapitel finden Sie eine Übersicht über die wichtigsten Funktionen.

### Voraussetzungen

* Im Menü **Plugin » Plugin-Übersicht** muss die Einstellung **Automatisch bereitstellen** aktiviert sein.
* Alle Plugins müssen bereits einmal in **Stage** bereitgestellt worden sein.

### Wichtige Informationen

* Nur Open-Source-Plugins, die nicht per Git in Ihrem plentymarkets System installiert wurden, werden synchronisiert.
* Von der automatischen Bereitstellung sind folgende Dateien ausgeschlossen:
 * Alle Dateien im Ordner **resources/libs**
 * Migrationen
* Verbotene Dateiänderungen werden geloggt und eine Warnung wird angezeigt.
* Der Ordnername eines neuen Plugins muss mit dem Plugin-Namen übereinstimmen.
* Plugin-Dateien können per `.gitignore` von der Synchronisierung ausgeschlossen werden.

### Plugins mit plentyDrive bereitstellen

1. Richten Sie plentyDrive wie oben beschrieben ein.
2. Nehmen Sie Änderungen an Ihrem Plugin im lokalen Ordner vor.
<br />→ plentyDrive bemerkt Dateiänderungen und kopiert die betroffenen Dateien in Stage.
<br />→ Ihre Änderungen sind sofort im Browser sichtbar.

### Terra-Vorschau

Beim Erstellen einer neuen Backend-UI gibt bisher keine Möglichkeit diese zu testen. Mit plentyDrive, können Sie Ihre Backend-UI nun mit plentyDrive-Geschwindigkeit testen.

1. Klicken Sie im Menü von plentyDrive auf **Terra-Vorschau öffnen**.<br />→ Ein emuliertes Chrome-Fenster wird geöffnet. plentyDrive verwendet die Login-Session des Systems und leitet alle Requests via CORS weiter.
2. Nehmen Sie Änderungen an Ihrem Plugin im lokalen Ordner vor.
<br />→ plentyDrive bemerkt Dateiänderungen und kopiert die betroffenen Dateien in Stage.
<br />→ Ihre Änderungen sind sofort im Browser sichtbar.
