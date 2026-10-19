# Exercise 7: Introduction to CI and Jenkins

## Continuous Integration (CI)
Developers push code to a shared repository often. A CI server detects each
push, builds the code, runs automated tests and reports the result, so errors
are found early.

## Jenkins
Jenkins is an open-source automation server used to build, test and deploy
software. Key concepts: job/project, build, pipeline, plugins, nodes.

## Install Jenkins with Docker
docker run -d --name jenkins -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts

## Get the initial admin password
docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword

## Access
http://localhost:8080 (8080 = web interface, 50000 = agent communication)

Screenshots: exercise7-unlock.png, exercise7-dashboard.png
