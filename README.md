# rpi-provisioning

Provision Arch Linux on the Raspberry Pi with Ansible. Just:

    cp hosts.example hosts

Edit the `hosts` file and:

    pip install -r requirements.txt
    ansible-playbook rpi-init.yml --ask-pass
