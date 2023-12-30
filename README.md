# cpanel-reconfigure

install ansible on a linux machine(literally any with an internet connection)

your package manager will probably have a version

apt install ansible

yum install ansible

dnf install ansible

pacman -Syy ansible

zypper in ansible

if not follow this guide to install with pip
https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html


```git clone https://github.com/Expand-sys/cpanel-reconfigure```

```cd cpanel-reconfigure```

Edit `inventory` to be the ipaddress of your cpanel server or 127.0.0.1 iof running locally

Edit `vars/default.yml` to have your chosen domain name and your email for ssl certs

```ansible-playbook -i inventory main.ansible.yml -k```

The requested password is the root password of the machine you are connecting to.
