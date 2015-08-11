
# [fit] **DevOps** Toolkit

---

# **Git**
####Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

### http://www.git-scm.com

---

![left fit](http://www.git-scm.com/images/assurance@2x.png)

### Distributed
### Small and Fast
### Staging Area -> **git commit -a**
### Encouraged to have multiple local branches
### Easy Merges

---

# **Git Commands**

####git add .

####git commit -am "Enter in a message here"

####git push

#### To **learn more** check out: GoTeaLeaf.com/books/git

---

![inline](https://www.prestashop.com/blog/en/files/2014/06/github-logo.png)
###Web-based Git repository hosting service

---

![fit](https://www.seedprod.com/wp-content/uploads/2015/05/Github-Search-Box-404-Page-Screenshot-Tiny-800x456.png)

---

![fit inline](http://tzookb.com/wp-content/uploads/2015/01/vagrant.png)

##Creates and configures virtual development environment

---

# **Vagrantbox.es**

###vagrant box add {title} {url}
###vagrant init {title}
###vagrant up

---

![fit](http://kappataumu.com/uploads/packer_splash.jpg)

---

#The **Template**
###example.**json**

````json
{
  "variables": {
    "aws_access_key": "",
    "aws_secret_key": ""
  },
  "builders": [{
    "type": "amazon-ebs",
    "access_key": "{{user `aws_access_key`}}",
    "secret_key": "{{user `aws_secret_key`}}",
    "region": "us-east-1",
    "source_ami": "ami-de0d9eb7",
    "instance_type": "t1.micro",
    "ssh_username": "ubuntu",
    "ami_name": "packer-example {{timestamp}}"
  }]
}
````

![right fit](https://packer.io/assets/images/screenshots/works_with-a1a499d3.png)

---

#**VMware** Example
```json
{
           "type": "vmware-iso",
           "iso_url": "{{user `iso_url`}}",
           "iso_checksum": "{{user `iso_checksum`}}",
           "iso_checksum_type": "{{user `iso_checksum_type`}}",
           "http_directory": ".",
           "boot_wait": "5s",
           "boot_command": [
               "<enter><wait10><wait10>",
               "/usr/bin/curl -O http://{{.HTTPIP}}:{{.HTTPPort}}/install-vmware.sh<enter><wait5>",
               "/usr/bin/curl -O http://{{.HTTPIP}}:{{.HTTPPort}}/poweroff.timer<enter><wait5>",
               "/usr/bin/bash ./install-vmware.sh<enter>"
           ],
           "disk_size": 20480,
           "ssh_username": "root",
           "ssh_password": "vagrant",
           "shutdown_command": "systemctl start poweroff.timer"
       }
```

---

![inline](https://www.cloudfoundry.org/wp-content/uploads/2015/06/Logo_CloudFoundry_Horizontal_HighRes1.png)

#**An Open Source** cloud computing platform as a service **(PaaS)**

---

![fit](http://ig.obsglobal.com/wp-content/uploads/2013/07/cloudfoundry_structure.png)

---

![fit](http://kpcbweb2.s3.amazonaws.com/companies/542/logo/original/slack-logo_large.png)

---

##Recommended Reading

![inline fit](https://puppetlabs.com/wp-content/uploads/2012/12/The-Phoenix-Proect-A-Novel-about-IT-DevOps-and-Helping-your-Business-Win.png)

---

##Recommended Reading

![inline](http://akamaicovers.oreilly.com/images/9780978739218/lrg.jpg)

---

##Recommended Reading

![line](http://akamaicovers.oreilly.com/images/0636920033158/lrg.jpg)

---

#[fit] **Thank** You!

### **Contact:** Richard.McGrath@EMC.com
### **GitHub:** Github.com/Rich-McGrath
