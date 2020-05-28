Máquina: devops
---------------

Procedimentos: 
--------------

* **Documentação Puppet**: https://puppet.com/docs/puppet/

* **Like Debian - Ubuntu**
  ```bash
  wget https://apt.puppetlabs.com/puppet6-release-bionic.deb
  dpkg -i puppet6-release-bionic.deb
  apt update && apt install puppetserver	
  ```

* Like RedHat
  ```bash
  rpm -Uvh https://yum.puppet.com/puppet6-release-el-7.noarch.rpm
  yum install puppetserver	
  ```

