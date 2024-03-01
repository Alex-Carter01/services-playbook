# services-playbook
Project for Vyopta showing an Ansible playbook remove, install, configure, and enable services

My process: 
- setup an EC2 instance with ubuntu-jammy-22.04-amd64-server-20240207.1

I am sshing with ubuntu-server-keypair.pem, this information is added to the included Ansible inventory file (hosts)

The playbook yaml then 
- [X] Removes the chronyd service if it's installed.
- [X] Removes the ntpd service if it's installed.
- [ ] Installs the systemd-timesyncd service.
- [ ] Configures the systemd-timesyncd via template.
- [ ] Enables and starts the systemd-timesyncd service.

