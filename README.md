
##  1. Pull Jenkins Image

docker pull jenkins/jenkins:lts-jdk17


## 2. Run Jenkins in Docker
docker run --user root -p 8080:8080 -p 50000:50000 \
--restart=on-failure -d \
-v /var/run/docker.sock:/var/run/docker.sock \
-v jenkins_home:/var/jenkins_home \
--name jenkins-docker \
jenkins/jenkins:lts-jdk17

## 3.install Dockers
apt update && apt install -y docker.io

## 4.in jenkins Dashboard add credentials 
    

## 5. inn pipelines item type create new items 
configurations as shown below
![image](https://github.com/user-attachments/assets/9269a7f9-1983-408d-9151-9e40e137e5d4)

![image](https://github.com/user-attachments/assets/8f0a2111-3a8e-41be-ba89-51bbc8b3b3a2)
![image](https://github.com/user-attachments/assets/3ae5b878-b0ed-4f7d-bf31-8e765f31e850)

