# Configuring VPN auto-connect on system startup on Linux

>nmcli connection show

## In this list, you need to find the type of your actual Internet connection, e.g., "Wired connection 1", and the UUID number of your current VPN connection.

>nmcli connection edit "Wired connection 1" 

>set connection.secondaries *insert your VPN UUID* and press Enter

>print connection.secondaries to check this out

>save

>quit
