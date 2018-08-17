# Setup my Raspberry Pi
This will do the following
- Add my user and ssh key
- Install Unifi Controller

TODO:
- Google Print Connector
- PiHole?

## Setup
Install ansible

```bash
brew install ansible
```

Fetch roles from Galaxy

```bash
ansible-galaxy install andrewrothstein.sudoers
```

## Usage
Bootstrap (Add my user)

```bash
ansible-playbook bootstrap.yml -u pi -k -b
```

Everything else

```bash
ansible-playbook main.yml -b
```