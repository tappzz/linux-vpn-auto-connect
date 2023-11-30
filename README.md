Configuring VPN auto-connect on system startup on Linux
nmcli connection show
nmcli connection edit e.g. "Wired connection 1" 
set connection.secondaries your VPN UUID
