# Jenkins Pipeline Job With Docker Integration


- This project demonstrates a Jenkins Pipeline Job that performs the following tasks:

- Connects Jenkins to a GitHub repository via webhook

- Builds a Docker image from a Dockerfile

- Runs a container using the built image

- Serves a static index.html page inside the container

All Docker commands are executed from within Jenkins (Docker-in-Jenkins)

## 📁 Project Structure


.
├── Dockerfile
├── index.html
├── docker.sh
└── README.md


## 🔧 Technologies Used
Jenkins (running on WSL2 Ubuntu)

Docker (configured inside Jenkins)

GitHub (SCM integration)

ngrok (to expose localhost for webhook testing)

## ✅ Prerequisites 


-  installed and running on port 8081

- Docker installed and accessible to Jenkins (e.g., Jenkins user in docker group)

- GitHub repository set up

- GitHub Personal Access Token (for push access)

- ngrok installed (to test webhooks from GitHub)

## PROJECT STEPS

1. Create the project Directory.

![directory](image.png)

2. Navigate to the Jenkins Home page to configure my first Jenkins Pipeline Job.

![home](image-1.png)

3. Get to the New Page select new item and then select Pipeline.

![new item](image-2.png)

4. General configurations, git url config etc

![gen](image-3.png)

![config](image-4.png)

5. Configure Trigger with hub Scm

![Trigger](image-5.png)

6. configure the pipeline Script.

![script](image-6.png)

7. Then we go to Pipeline Syntax to configure the pipeline script

![syntax](image-7.png)

8. Then add the github repository that is configured to the overview page, then the github branch.

![hub config](image-8.png)

9. Then generate the Pipeline Script and add it to the pipeline script.

![script](image-9.png)

10. Then i install docker on the Jenkins instance.

![docker](image-10.png)

11. create a docker.sh file, create Dockerfile, and make it executable.

![docker.sh](image-11.png)

![exe.](image-12.png)

12. check docker status, then write an nginx script for docker image and index.html.

![status](image-13.png)

![nginx](image-14.png)

![index.html](image-15.png)

13. Login to Github to create a webhook, go to settings sellect webhook, add payload url, and then add webhook.

![github repo](image-16.png)

![webhook](image-17.png)

![payload](image-18.png)

14. then add a webhook.

![webhook](image-19.png)

15. usermod

![usermod](image-20.png)

![push to github](image-21.png)

16. build successful.

![build](image-22.png)

![build graph](image-23.png)

17. welcome to Pipeline Job.

![job](image-24.png)

# PROJECT CONCLUDED





