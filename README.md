# wireguard_setup

    sudo apt install wireguard-tools resolvconf

copy the conf file to /etc/wireguard dir

    sudo su
    cp <name>.conf /etc/wireguard

wireguard up 

    sudo wg-quick up <name>.conf
    sudo wg-quick save <name>

for wireguard to be automatically up, everytime you turn on your system

    sudo systemctl enable wg-quick@<name>
