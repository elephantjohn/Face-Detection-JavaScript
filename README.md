# IMPORTANT: Bug Fixes

## `navigator.getUserMedia`

`navigator.getUserMedia` is now deprecated and is replaced by `navigator.mediaDevices.getUserMedia`. To fix this bug replace all versions of `navigator.getUserMedia` with `navigator.mediaDevices.getUserMedia`

## Low-end Devices Bug

The video eventListener for `play` fires up too early on low-end machines, before the video is fully loaded, which causes errors to pop up from the Face API and terminates the script (tested on Debian [Firefox] and Windows [Chrome, Firefox]). Replaced by `playing` event, which fires up when the media has enough data to start playing.

## how to run
use Live Server with VSCode.     
how to install LiveServer in vscode?    
Launch VS Code Quick Open (Ctrl+P), paste the following command, and press enter.   
```
ext install ritwickdey.LiveServer   
```
Open a HTML file and right-click on the editor and click on Open with Live Server.   
or Hit (alt+L, alt+O) to Open the Server and (alt+L, alt+C) to Stop the server (You can change the shortcut form keybinding). [On MAC, cmd+L, cmd+O and cmd+L, cmd+C]  

see [here](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) for more info
