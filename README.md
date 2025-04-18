# Docker1
docker jenkens k6 sonar added to test

Tools:

1. Kubernetes Cluster - container orch
2. Docker - runtime
3. Jenkins- CICD server
4. DockerHub - container reg
5. helm - packaging & deploy on k8
6. git - version control repo
7. Maven - Build Tool
8. SonarQube - code analysis server


###############################################################

Flow of execution

1. Ci setup   - jenkins, sonarcloud (nexus)
2. Dockerhub acct
3. Store dockerhub acct credentials in jenkins
4. Setup docker engine in jenkins
5. Install plugins in jenkins 
    a.docker-pipeline  b.docker  c.pipeline util
6. Crete kubernetes Cluster with Kops
7. Install helm on the Kops VM
8. Create Helm charts
9. Test charts in k8 cluster in test namespace
10. Add Kops VM as jenkins slave
11. Createpipeline code [declarative]
12. Update git repo with:
    a. helm charts  b. Dockerfile  c. jenkinsfile (pipeine code)
13. Create Jenkins job for pipeline
14. Run and test job

