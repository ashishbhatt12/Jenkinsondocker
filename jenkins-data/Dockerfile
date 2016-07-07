FROM debian:jessie
MAINTAINER Ashish Bhatt

# Create the Jenkins user in this container 
RUN useradd -d "/var/jenkins_home" -u 1000 -m -s /bin/bash jenkins

# Create log file
RUN mkdir -p /var/log/jenkins
RUN chown -R jenkins:jenkins /var/log/jenkins

# Docker volume magic
VOLUME ["/var/log/jenkins", "/var/jenkins_home"]

USER jenkins

CMD ["echo", "Data container for Jenkins 2.0"]