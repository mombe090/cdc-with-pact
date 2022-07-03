FROM jenkins/jenkins:2.357

# Install required plugins
RUN jenkins-plugin-cli --plugins git:4.11.3
RUN jenkins-plugin-cli --plugins blueocean:1.25.5
RUN jenkins-plugin-cli --plugins --plugins job-dsl:1.79

# Skip initial setup
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
