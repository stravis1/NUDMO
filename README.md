# NUDMO  Nginx-Uwsgi-MySQL-OpenStack

### Overview.
Done as an educational project to provide a simple ansible setup for configuring existing  VMs in OpenStack.

## SETUP: Prerequisits:

- The method leverages the Vagrant methodology and expects that you have launched your VMs from Vagrant.  Thus the /vagrant directory is available on the VMs to supply needed configuration files for nginx and django. 

- The ansible script expects 3 VMs to be setup.
    1. A web front end to run nginx, uwsigi and django
    2. A db server for mysql
    3. A ansible server.
- Make sure your web, db and ansible servers have the correct ssh keys needed by ansible. 

Step 1:
- on the Ansible server: Clone the repo: (git clone https://github.com/nudmo)
- Add the web server and the db server to the hosts file.

Step 2: Run ansible
 - ansbile-playbook ./site.yml -i ./hosts


