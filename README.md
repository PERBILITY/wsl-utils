# wsl-utils
Some utilties for developers working and developing with WSL.

## Startscripts for PhpStorm / WebStorm
The files `phpstormd` and `webstormd` in the folder `jetbrains` are startscripts for PhpStorm/WebStorm, that run the respective IDE 
in background with output handling.<br>
By default the scripts have logging enabled which means the `stdout` and `error` outputs are saved in separate log files
under `~/logs/PhpStorm/` / `~/logs/WebStorm/` with a filename that includes the date and time of when the script is executed.<br>
The created log files will be saved for 3 days and autodeleted by the script on the 4th day.<br>
You can change the default behaviour by editing the variables on the top of the script.

For installation run the respective command for your IDE in WSL:<br>
**WebStorm**<br>
`wget -O ~/bin/webstormd https://raw.githubusercontent.com/PERBILITY/wsl-utils/main/jetbrains/webstormd && chmod +x ~/bin/webstormd`<br>
**PhpStorm**<br>
`wget -O ~/bin/phpstormd https://raw.githubusercontent.com/PERBILITY/wsl-utils/main/jetbrains/phpstormd && chmod +x ~/bin/phpstormd`

**Hint**<br>
To start the IDE directly from Windows you can create a new shortcut and set the target 
to `C:\Windows\System32\wsl.exe bash -li <startscript>` where `<startscript>` has to be replaced by the respective script. 
(either `phpstormd` or `webstormd`)


