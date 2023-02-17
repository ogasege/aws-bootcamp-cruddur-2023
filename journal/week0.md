# Week 0 — Billing and Architecture

This weeek, I was able to complete my homework without any issue. 
For my assignment challenges, I:
## Watched Week 0 - Live Streamed Video
I learnt about how it is to work on projects in the real world from the characters in the scenario used during the livestream. I also learnt about the iron triangle and how it applies to various projects depending on the objectives. 

## Watched Chirag's Week 0 - Spend Considerations
I understood the free tier plan that AWS offers and I will ensure that I conider the costs pf resources before I use them during the course of this bootcamp as well as in other projects. 

## Watched Ashish's Week 0 - Security Considerations
I understand the part I have to play as a cloud engineer in ensuring that I ensure that best practices for security are always employed and I got more eye openers as I watched this video. 

## Recreated Conceptual Diagram in Lucid Charts and on a Napkin
Using a napkin, I made this conceeptual diagram. I added features such as crud alarms, crud backups as well as crud scheduling (twitter killer indeed👌😉) 

![PHOTO-2023-02-15-16-46-56](https://user-images.githubusercontent.com/87014766/219663317-7645514a-04b0-4613-bffe-7f0d61eca466.jpg)

The conceptual design was recreated on Lucid Chart. 

![Cruddur](https://user-images.githubusercontent.com/87014766/219663695-270d1471-4c95-4031-8eed-63b48fb0bfbd.png)

It can be found here [Conceptual Design of Cruddur](https://lucid.app/lucidchart/3f0ec92f-4488-4daf-a436-d24272353ec0/edit?viewport_loc=-296%2C-124%2C2556%2C1352%2C0_0&invitationId=inv_df73616d-9114-4456-a54a-12fdaddddf6f) 

## Recreated Logical Architectural Diagram in Lucid Charts
I also recreated the logical architectural diagram given using Lucid Charts. 
![Cruddur Logical Diagram](https://user-images.githubusercontent.com/87014766/219664850-5b43678b-ba1f-4dfc-8247-3f9079665789.png)

It can be found here
[Logical Architecture Diagram of Cruddur](https://lucid.app/lucidchart/5d19199a-c5e8-43c1-8a62-0085f2f63d9c/edit?viewport_loc=-175%2C131%2C2556%2C1352%2C0_0&invitationId=inv_3fc743ed-b8a1-40fc-939e-0ff30d6dd4c5) 

## Created an Admin User
I created an admin user which will be used for the bootcamp to comply with best practices of not using your root user except for very specific tasks.

## Used Cloudshell

## Generated AWS Credentials

## Installed and used AWS CLI 

The used AWS CLI commands can be found below:
```
tasks:
  - name: aws-cli
    env:
      AWS_CLI_AUTO_PROMPT: on-partial
    init: |
      cd /workspace
      curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
      unzip awscliv2.zip
      sudo ./aws/install  
      cd $THEIA_WORKSPACE_ROOT
vscode:
  extensions:
    - 42Crunch.vscode-openapi
```


## Created a Budget and a Billing Alarm
I created a $1 dollar budget and set up a billing alarm using 80% of the chosen metric as the threshold. I created the budget using the AWS CLI commands and used the management console to set up the billing alarm. 

## Created an SNS topic
I created an SNS topic and subscribed using my mail address provided.
![image](https://user-images.githubusercontent.com/87014766/219659772-4b3c7ebe-6713-47b2-b49e-493e9b466ccd.png)


