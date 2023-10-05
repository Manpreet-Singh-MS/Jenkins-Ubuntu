Java JRE Installation
=====================

<code>sudo apt-get install openjdk-11-jre</code>

<code>java --version</code>


Jenkins Debian Packages
=======================

This is the Debian package repository of Jenkins to automate installation and upgrade. To use this repository, first add the key to your system :-

<code> curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
    /usr/share/keyrings/jenkins-keyring.asc > /dev/null </code>

Then add a Jenkins apt repository entry :-

<code>echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
    https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
    /etc/apt/sources.list.d/jenkins.list > /dev/null </code>

Update your local package index, then finally install Jenkins :-

<code>sudo apt-get update</code>

<code>sudo apt-get install fontconfig openjdk-11-jre</code>

<code>sudo apt-get install jenkins</code>

Check the status of Jenkins
===========================

<code>sudo systemctl enable jenkins</code>

<code>sudo systemctl start jenkins</code>

<code>sudo systemctl status jenkins</code>
