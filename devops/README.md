# DevOps Study Guide
* [Topics](#topics)
* [Practice projects](#practice-projects)
* [Resources](#resources)

# Topics
TBD

# Practice projects
### Create users
- Create user devopsadmin
- Create group devops
- Add devopadmin to devops group
- Provide devops with passwordless sudo access
- Create ssh keys

- Create user devopsreadonly
- Create group devopsread
- Add devopadreadonly to devopsread group
- Switch user to devopsreadonly
- Try to sudo
- Provide log to show user tried to sudo
- Create ssh keys

### Basic security
- configure ufw or iptables to allow ssh access from your current IP address

### Subnetting
- What is /32?
- What is /8, /16,/24?


### Shared directory
- On your native OS create dir called devopsshared
- Share devopsshared on your VM

### Scripting
Write a script to:
- create 30 sub-dirs in devopsshared
    - name devopsshared_01 - 30
- create 5 files in every sub-dir (devopsshared_01_file1.txt)
- create devopsshared_backup in devopsshared

Your script will grab devopsshared_0*_file1.txt, file3.txt and file5.txt, then in every directory it needs to be zipped first then moved into devopsshared_backup then zipped again with devopsshared_backup_<current _date>

### Software installation
- Install Apache or Nginx
- Create a website called devops.com
- Create site to publish "hello world"
- Configure custom logs called
    devops_access
    devops_error

- Configure logs to rotate and compress weekly

- Setup self-signed ssl certificate that will expire 2020
- What do you need to do with ufw?
- Bonus: have nginx forward to apache

# Resources

- https://linuxize.com/

- https://www.digitalocean.com/community/tutorials/

- https://www.youtube.com/playlist?list=PLS1QulWo1RIb9WVQGJ_vh-RQusbZgO_As

- https://www.youtube.com/playlist?list=PLS1QulWo1RIYmaxcEqw5JhK3b-6rgdWO_
