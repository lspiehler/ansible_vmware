# Example Ansible VMware Build with Kickstart and PXE/iPXE

* Install pyvmomi and python requests library
* Update vars.yml for your environment
* Update hosts with your tftp/http server

```
yum install python2-requests python2-pyvmomi

ansible-playbook -i hosts.yml -e @vars.yml build.yml
```