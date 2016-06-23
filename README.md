# Tomcat-Cluster-Load-Balancing

The steps are written assuming that the working machine is Ubuntu/Debian

=> Setting Up Ansible
1) Install Ansible: apt-get install ansible
2) Test the installtion by running: ansible all -m ping --ask-pass. If you get a prompt asking for the SSH password, it means that the installation was successful.
3) Add server IP or hostname inside /etc/ansible/hosts
4) Test if Ansible is able to reach the server by using: ansible all -m ping -u <server-username> --ask-pass. (Use the flag --private-key if using key-based authentication)

Note: You might need to install the utility sshpass: apt-get install sshpass

=> Running the Playbook
1) Download the playbook from the repo: setup.yml
2) Run with the following command: sudo ansible-playbook setup.yml
