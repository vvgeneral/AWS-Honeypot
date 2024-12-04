# Honeypot on AWS EC2 using TPOTCE  

## Project Overview

This project involves deploying a honeypot on an Amazon EC2 instance using TPOTCE. TPOTCE is an open-source honeypot framework that integrates multiple honeypot tools, enabling detection, logging, and analysis of malicious activity in a controlled environment.

The honeypot is designed to attract attackers by simulating vulnerable services, providing valuable insights into real-world attack techniques and patterns. I was able to detect attacks coming from all over the globe and at different times of the day. This data was then visualized using Kibana to display data graphically; you can see some of those pictures [here](./screenshots).

## What I Learned

Starting with AWS, I already had experience creating EC2 instances but never used SSH to connect to them. I would typically use the EC2 instance connect, so SSHing using a key pair got me comfortable with the process. Additionally, I gained a lot of valuable information on using security groups since I had to change the rules on them so much for this project.

As for other tools, this was my first time interacting with Kibana and creating visualizations like this. Moreover, I have never used honeypot tools, but I feel confident making and architecting honeypots after my experience building one. Since I used Debian for the EC2 instance, I am even better at the Linux command line interface.