# Jenkins With Docker

- Go to docker hub and search for jenkins.
- Make sure your docker is running before installation.
- Use the below command to install jenkins image in your docker.

```
docker run -p 8080:8080 -p 50000:50000 -d -v /your/home:/var/jenkins_home jenkins/jenkins:lts
```

- After installation default password is generated in CLI. Save it because you need during login process.
- Also the default password can be found under

```
$jenkins_home/secrets/initialAdminPassword

```

- The default username of jenkins is admin.
- Run `localhost:8080` in your browser and login with default username and password to work with jenkins.
- Install suggested plugins at the beginning but different plugins are needed depending upon application and version control used.
- Create first admin user.
- Jenkins Dashboard appears.
