# IaC for rPi Ditto/SenseHat Nodes

## Setup the Inventory

Edit the `inventory.ini` with the appropriate details for the target RaspberryPi devices

## Deploy

`ansible-playbook -i pi1, --ask-vault-pass --ask-become-pass site.yml`

or specific tags

`ansible-playbook -i pi1, --ask-vault-pass --ask-become-pass --tags ditto_bluez site.yml`


## TODO

### Install EI

https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-cpu-gpu-targets/raspberry-pi-4#2.-installing-dependencies
```bash
sudo apt install -y gcc g++ make build-essential nodejs sox gstreamer1.0-tools gstreamer1.0-plugins-good gstreamer1.0-plugins-base gstreamer1.0-plugins-base-apps
npm config set user root && sudo npm install edge-impulse-linux -g --unsafe-perm
```
