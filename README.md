# IaC for rPi Ditto/SenseHat Nodes

## Setup the Inventory

Edit the `inventory.ini` with the appropriate details for the target RaspberryPi devices

## Deploy

`ansible-playbook -i pi1, --ask-vault-pass --ask-become-pass site.yml`

or specific tags

`ansible-playbook -i pi1, --ask-vault-pass --ask-become-pass --tags ditto_bluez site.yml`

