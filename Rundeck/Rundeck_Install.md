Máquina: automation
-------------------

Procedimentos:
--------------

* **Documentação Rundeck:** https://docs.rundeck.com/

* Like Debian
  ```bash
  apt-get install openjdk-8-jdk-headless
  wget https://dl.bintray.com/rundeck/rundeck-deb/rundeck_3.1.0.20190731-1_all.deb
  dpkg -i rundeck_3.1.0.20190731-1_all.deb
  ```

* Like RedHat
  ```bash
  yum install java-1.8.0
	rpm -Uvh https://repo.rundeck.org/latest.rpm
  yum install rundeck
  ```
