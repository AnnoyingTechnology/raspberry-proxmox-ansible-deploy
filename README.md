# raspberry-proxmox-ansible-deploy
Configure multiple freshly installed Raspberry as working Proxmox 8+ nodes.

It assumes
- that you have paired your public key using rpi-imager (don't create an account, just set your public key).
- that you have assigned prefered IPs using MAC addresses on you DHCP server. 

The playbook will then
- assign those IP permanently as static IP.
- configure the nodes completely, with a working PVE on it.

All that remains after running the playbook, it to make them join the same cluster. 

**DISCLAIMER** the proxmox for ARM64 resposity is maintained by a single China resident. He is either extremely generous (and I thank him for providing the repository) or state sponsored to inject backdoors. It's up to you to trust or not this repo. You may want to set router's firewall rules accordingly.
