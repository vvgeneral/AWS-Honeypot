# Honeypot on AWS EC2 using TPOTCE  

## Project Overview

This project involves deploying a honeypot on an Amazon EC2 instance using TPOTCE. TPOTCE is an open-source honeypot framework that integrates multiple honeypot tools, enabling detection, logging, and analysis of malicious activity in a controlled environment.

The honeypot is designed to attract attackers by simulating vulnerable services, providing valuable insights into real-world attack techniques and patterns. I was able to detect attacks coming from all over the globe and at different times of the day. This data was then visualized using Kibana to display data graphically; you can see some of those pictures [here](./screenshots).

## What I Learned

Starting with AWS, I already had experience creating EC2 instances but never used SSH to connect to them. I would typically use the EC2 instance connect, so SSHing using a key pair got me comfortable with the process. Additionally, I gained a lot of valuable information on using security groups since I had to change the rules on them so much for this project.

As for other tools, this was my first time interacting with Kibana and creating visualizations like this. Moreover, I have never used honeypot tools, but I feel confident making and architecting honeypots after my experience building one. Since I used Debian for the EC2 instance, I am even better at the Linux command line interface.

Outside of tools and technologies, I got to see for myself some attack patterns! For example, this one attacker kept trying to brute force the SSH each second for hours, and I could see them using stuff like 001000, 111100, 001234, 001230, etc. A polar opposite of this attacker was one that only tried 3 times and then stopped permanently. An attacker in the middle of the spectrum between these two would try 3 times, wait 5 minutes, then try 3 times again. I was also able to see Suricata signatures, the most common one being 2210051 “SURICATA STREAM Packet with broken ack."