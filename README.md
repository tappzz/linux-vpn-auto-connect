# Configuring VPN auto-connect on system startup on Linux

>nmcli connection show

### In this list, you need to find the name of your actual Internet connection, e.g., "Wired connection 1", and the UUID number of your current VPN connection.

>nmcli connection edit "Wired connection 1" 

>set connection.secondaries *insert your VPN UUID* and press Enter

>print connection.secondaries to check this out

>save

>quit

Reboot your PC

If you want to roll back these settings, you should open the nmcli menu again and change the connection.secondaries by typing the following lines:

>nmcli connection edit "Wired connection 1" 

>set connection.secondaries *leave this field empty* and press Enter

>save

Then you could type the following line to check this out:

>print connection.secondaries 

>quit


