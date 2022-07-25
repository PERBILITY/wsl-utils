# wsl-utils
Some utilties for developers working and developing with WSL.

## Startscripts for PhpStorm / WebStorm
The files `phpstormd` and `webstormd` are startscripts for PhpStorm/WebStorm, that can be used to create Windows shortcuts for theese IDE's.<br>
By default the scripts have logging enabled and save the log files under `~/logs/PhpStorm/` / `~/logs/WebStorm/` with a filename that includes the date and time of when the script is executed.<br>
The created log files will be saved for 3 days and autodeleted by the script on the 4th day.<br>
You can change the default behaviour by editing the variables on the top of the script.<br>

For installation see the respective instructions for your IDE below.
### WebStorm
- Run the following Command in WSL:<br>
`wget -O ~/bin/webstormd https://raw.githubusercontent.com/PERBILITY/wsl-utils/main/webstormd && chmod +x ~/bin/webstormd`
- In Windows create a new shortcut with target `C:\Windows\System32\wsl.exe bash -li webstormd`

### PhpStorm
- Run the following Command in WSL:<br>
`wget -O ~/bin/phpstormd https://raw.githubusercontent.com/PERBILITY/wsl-utils/main/phpstormd && chmod +x ~/bin/phpstormd`
- In Windows create a new shortcut with target `C:\Windows\System32\wsl.exe bash -li phpstormd`


