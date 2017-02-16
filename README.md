# ansible_lab
Playground for Ansible

v0.3.0
 - Added mysql role (Currently without connection to nginx)
   - install mysql
   - create DB named lab
   - Create table users
   - Enter first entry
   - Create webuser user

v0.2.0
 - Changed Ansible to work with roles insted of flat playbook
 - Changed inventory "allservrs" to "common"
 - Removed unused files

v0.1.0 First version:
 - Ansible with basic deployment of one HAProxy server and 2 Nginx servers
 - HAProxy loadbalance 2 Nginx servers
   - Haproxy installed and running on port 80
   - Load balances requests to Test2 and Test3 port 8000
   - Failover for hosts Test2 and Test3 should be setup for port 8000
 - Nginx servers with basic configuration:
   - Nginx is installed and running on port 8000
   - The file "/var/www/local.html" exists and contains the hostname of each machine
   - Nginx location rules as following:
     - "/probe_local" should show the contents of /var/www/local.html
     - "/probe_applicant" should return your availability for being 24/7 on-call at CeleraOne (shared with other team members)
     - "/*" forwarded to your favorite website
     - "/probe_remote" forwarded to localhost:5500


