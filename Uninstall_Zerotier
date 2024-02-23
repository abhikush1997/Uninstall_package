#!/bin/bash

### Remote server details
USER_ID="username"
IP_ADDRESS="remote_server_ip"
PASSWORD="key"

### Software details to Uninstall
software_NAME="Zerotier"

### Connect to the remote server using SSH
ssh "$USER_ID@$IP_ADDRESS" <<END

    ### Use the package manager to uninstall the software
    sudo apt-get remove $software_NAME

    ### Remove configuration files
    sudo apt-get purge $software_NAME

    ### Update the package list
    sudo apt-get update

    exit
END
