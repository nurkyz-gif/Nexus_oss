<<<<<<< HEAD
# Nexus3-1.
***Nexus*** is an open source repository manager that allows you to proxy , collect and manage your  dependencies. It supports many artifact formats including Java.
Then we take these binaries that are already uploaded in nexus to ansible playbook. Ansible Playbook is a YAML file integrated in the application code , then deploys it to the CentOS machine.
We have downloaded our roles from Ansible Galaxy and run them in the Ansible Playbook.
Our app is opening from https. Https is a secure version of the http protocol that uses the ssl/ls protocol for encryption.  
**Pre-requisites:**
- git
- httpd (apache)
- openjdk (Java-1.8.0- nexus runs on Java language)
- wget (to download  configurations for nexus)
- openssl (created self signed certificate). 
**Languages:**.
Java-1.8.0.
**Set:**
Selinux= disabled.
**Roles:**
```
  - name: Install OpenJDK.
    import_role:
      name: ansible-role-openjdk.
  - name: Apache proxy vhost.
    import_role:
       name: ansible-apache-vhost.
  - name: SSL Selfsigned.
    import_role:
      name: ansible-ssl-selfsigned.
  - name: Nexus.
    import_role:
      name: ansible-role-nexus3.
```
**License**
MIT License  
=======
# nexus_oss
>>>>>>> 9eff486dcd5aa8fc3e9abeb61b820f3363312f39
