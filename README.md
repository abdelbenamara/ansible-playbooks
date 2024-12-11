# ansible-playbooks

## Setup

```
sudo apt update
sudo apt install python3 python3-pip python3-venv
python3 -m venv venv
source venv/bin/activate
pip install --upgrade pip
pip install --upgrade setuptools wheel
pip install --upgrade ansible-core
ansible-galaxy collection install --upgrade community.general
```

## Usage

- Access Management for Debian
```
ansible-playbook access-management-debian.yml [--ask-become-pass] [--extra-vars '{"ssh_port":<number>}']
```

- AdGuard Home for Debian
```
ansible-playbook adguard-home-debian.yml [--ask-become-pass] [--extra-vars '{"home_port":<number>,"dns_port":<number>,"tmp_dir":"<path>"}']
```

- PiVPN Wireguard for Debian
```
ansible-playbook pivpn-wireguard-debian.yml [--ask-become-pass] [--extra-vars '{"vpn_user":"<username>","vpn_port":<number>,"tmp_dir":"<path>"}']
```
