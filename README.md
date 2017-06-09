# xmpp.dk ansible setup

Preparing to move xmpp.dk to new hardware. To ease the process, everything will be 
configured using Ansible to: 

 * Install the required base system
 * Install Prosody including extra modules
 * Download and restore the latest remote backup
 * Install nginx
 * Download and install the website

To run: 

 * Acquire a fresh Debian Jessie server. Python should be available for Ansible to run. 
 * On your Ansible controller :`ansible-playbook -i staging all.yml  --ask-vault-pass`