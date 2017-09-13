# Introducing plentyDrive

The new plentymarkets tool plentyDrive offers the functionality to skip time-consuming plugin builds by synchronising your local inbox with your system's preview mode stage.

## Installing plentyDrive

Click the link for your operating system and follow the respective installation routine.

## Configuring plentyDrive

Follow these steps to complete the setup of plentyDrive.

1. Open plentyDrive.
2. Enter your plentymarkets domain.
3. Enter your login data.
4. Click on **Login**.<br />→ plentyDrive is logged into your system.
5. Click on **Settings**.
6. Select a local folder to be synchronised with the plugin inbox.
7. **Save** the settings.<br />→ plentyDrive will restart.<br />→ The configuration is complete.

## Using plentyDrive

plentyDrive can greatly reduce the amount of time needed for applying changes to your plugins. This chapter will provide an overview of the main functions.

### Prerequisites

* **Deploy automatically** has to be activated in **Plugin » Plugin overview**.
* All plugins have to be deployed in **Stage** once.

### Important information

* Only open source plugins not installed via Git in your plentymarkets system will be synchronised.
* Excluded from autodeploy are:
 * all files in the folder **resources/libs**
 * migrations
* Forbidden file changes are logged and a warning is displayed.
* When creating new plugins, the folder name has to match the plugin name.
* You can exclude plugin files from synchronisation via `.gitignore`.

### Deploying plugins using plentyDrive

1. Configure plentyDrive as described above.
2. Make changes to your plugin in the local folder.
<br />→ plentyDrive recognises any file changes and copies the respective file into the stage directory.
<br />→ Your changes are immediately visible in the browser.

### Terra preview

When building a back end UI, there is currently no way to test it. With plentyDrive, you can not only test it, but do so with the same speed plentyDrive lends other plugins.

1. In the plentyDrive menu, click on **Open Terra preview**.<br />→ An emulated Chrome window will open. plentyDrive uses the login session of the system to forward all requests with CORS.
2. Make changes to your plugin in the local folder.
<br />→ plentyDrive recognises any file changes and copies the respective file into the stage directory.
<br />→ Your changes are immediately visible in the browser.
