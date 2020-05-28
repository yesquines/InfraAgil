Máquina: docker
---------------

Procedimentos:
--------------

* **Documentação GitLab:** https://docs.gitlab.com/

* **Docker Installation**
```bash
docker run -d --name gitlab -v gitlab_config:/etc/gitlab -v gitlab_data:/var/opt/gitlab -p 8080:80 --restart=always gitlab/gitlab-ce
```

* SO Installation
   - Like RedHat
   ```bash
   yum install -y curl policycoreutils-python openssh-server
   curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.rpm.sh | bash
   yum install -y gitlab-ce
   ```

   - Like Debian
   ```bash
   apt-get install -y curl openssh-server ca-certificates
   curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.deb.sh | bash
   apt-get install gitlab-ce -y
   ```
