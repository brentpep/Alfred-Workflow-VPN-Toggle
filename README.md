# [Alfred](http://www.alfredapp.com) Workflow VPN Toggle w/ Keyboard Shortcut

Alfred Workflow for Toggling a VPN connection with customizable keyboard shortcut.

Supports OS X 10.11 El Capitan

## Installation

Download and open file using [Alfred 2](http://www.alfredapp.com/).

You need to [buy the Powerpack](https://buy.alfredapp.com/) to use these workflows.

Download the .alfredworkflow file and open it.

## Usage

1. Open .alfredworkflow file
2. Edit the script to include your VPN settings
3. Customize the Hotkey to fit your needs. The set hotkey is currently `control+spacebar`.
4. Enjoy!

## Editing the Script

```
on alfred_script(q)
	set theConnection to "REPLACE" -- Change this to the name of your VPN connection
	set connectionWindowTitle to "VPN Connection"
	set theApp to "UserNotificationCenter"
	set thePassword to "REPLACE"
	open_vpn_connection(theConnection, thePassword, theApp, connectionWindowTitle)
end alfred_script
```