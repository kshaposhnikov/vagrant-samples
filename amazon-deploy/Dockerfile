FROM jenkins/jenkins:latest

COPY plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt


ADD JENKINS_HOME /var/jenkins_home/

USER root
RUN chown -R jenkins /var/jenkins_home/jobs/
RUN chmod -R 777 /var/jenkins_home/jobs/Petclinic/
