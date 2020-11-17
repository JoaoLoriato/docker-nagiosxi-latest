# About the image

This is a docker image containing Nagios XI Latest version, based on the official Nagios XI installer.

https://assets.nagios.com/downloads/nagiosxi/docs/Installing-Nagios-XI-Manually-on-Linux.pdf

Check my github repository for this project to see a Dockerfile. 

https://github.com/JoaoLoriato/docker-nagiosxi-latest

# Basic usage
docker run -d -p 80:80 --name nagios-xi joaoloriato/nagios-xi-latest

You'll be able to access Nagios' web interface once that goes up. As of default, there will be some local services already being monitored by Nagios. You can safely remove local NTPD and SSH service monitoring, since they are not included and not needed in this container build.

# Trial license
You can use Nagios XI with most of its features completely free for 60 days (see FAQ here). After that, go to 'license information' page and change the license type to free. Free version is limited and it allows you to monitor only up to 7 hosts.
