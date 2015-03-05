# rpi-provisioning

Provision Arch Linux on the Raspberry Pi with Ansible. Just:

    cp hosts.example hosts

Edit the `hosts` file and:

    pip install -r requirements.txt
    ansible all -m raw -a "pacman -S --noconfirm python2" -u root --ask-pass
    ansible-playbook rpi-init.yml --ask-pass
