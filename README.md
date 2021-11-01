# anslible
Playbooks for install: 
- nginx
- static page
- psql 

To install and configure NGINX run next:
add your host and user to inventory.yml
ansible-playbook -i inventory.yml nginx.yml

To setup static page run next:
ansible-playbook -i inventory.yml sync.yml
Open a web browser and test the website by going to
http://helloword.com

To setup postgresql with user and password, please run next playbook:
ansible-playbook -i db_install.yml
also please use -K parameter for your SSH private key
and -u for specifying a remote user

(all playbooks were sucsefylly installaed on AWS Ubuntu 20.04)
