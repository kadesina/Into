# Introduction 

  The Active Directory lab is focused on detecting unauthorized user activity. It includes creating alerts in Splunk, and integrating Slack and Shuffle for automated detection and response. The lab is deployed on the [Vultr cloud platform](https://www.vultr.com/) , providing a scalable and realistic environment for hands-on cybersecurity training.
I will be using this labs to get hands on skills learning splunk and shuffle, as i have never used any of these platforms before. Ill also be configuring a firewall within the cloud envuironmment whichwill also give me some networking experience within a SOC enviroment. 

- Part 1 (Building a logical diagram for visiaulaization)
  > This will help with understanding how the environment will look like.
    
- Part 2 (Setting up the cloud environment)
  > - Deploy windows server
  > - Deploy ubuntu server
- Part 3 (Install and Setup Active Directory)
  > In this part of the project, I will install Active Directory on my server and promote it to a Domain Controller. Additionally, I will join a computer to the domain and create several user accounts. To verify everything is working correctly, I’ll log in as one of the users and ensure proper authentication and domain functionality.
- Part 4 (Configure Splunk and Create Alerts)
  > In this part im going to configure and install splunk on an ubuntu server that ill be deplying on on vultr, then start ingesting telemetry from collected from windows enpoint. Then ill create an alert that detects unauthorized successful logins. 
- Part 5 (Integrate Slack & Shuffle for Automation)
  
  > The goal of this final phase is to create a small automation playbook for handling successful unauthorized login attempts. When such an event is detected:
  > - A notification will be sent to Slack
  > - An email will be sent to the SOC analyst, asking whether to disable the user account
  > - If the analyst replies "yes", the user will be automatically disabled
     
  > This workflow will be built using Shuffle and will simulate a real-world SOAR (Security Orchestration, Automation, and Response) process.


  
