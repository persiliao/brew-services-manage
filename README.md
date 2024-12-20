# brew-services-manage

> An macOS menu item for managing homebrew services.

This reads the [homebrew services](https://github.com/Homebrew/homebrew-services) command, showing you the status of your services and allowing them to be started, stopped and restarted.

<img src="docs/screenshot.png" alt="Screenshot" width="197">

## Install

### Manually

Download from the [Releases](https://github.com/persiliao/brew-services-manage/releases) page.

⚠️ You'll see a warning <cite>"**Brew Services Manage**" can't be opened because Apple cannot check it for malicious software</cite>. This is because I haven't paid Apple for a developer account.

[More info about this malicious software warning](https://support.apple.com/en-gb/guide/mac-help/mchleab3a043/mac).

### Autostart

The program doesn't have an option to autostart itself, so you may want to open **System Preferences** -> **General** -> **Login Items** and add the application to the list to have it start when you log in.

## Usage

The operation of the service is carried out by clicking the option of the secondary menu of the specified service

- **Run** Run the service
- **Start** Start the service and set it to auto-start at power-on
- **Restart** restart the service
- **Kill** Kill the service
- **Stop** Stop the service and unset it to auto-start at power-on
- **Log** Open the log file for the service, if one exists
- **Error Log** Open the error log file for the service, if one exists
- **Pin** Pin the service
- **Plist** Open the plist file for the service
- **Upgrade** Open the plist file for the service

> If you have installed a new service using another method (e.g. terminal), you need to click **Help** -> **Restart** to reload it

## Homebrew

By default looks for Homebrew at `/usr/local/bin/brew` and `/opt/Homebrew/bin/brew`.