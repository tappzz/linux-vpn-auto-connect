# Configuring VPN auto-connect on system startup on Linux

>nmcli connection show

>nmcli connection edit *e.g. "Wired connection 1"* 

>set connection.secondaries *insert your VPN UUID*

>print connection.secondaries to check this out

>save

>quit
