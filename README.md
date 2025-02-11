GAME DAY NOTIFICATION/SPORT ALERT SYSTEM

PROJECT OVERVIEW

This project is an alert system that sends real-time NBA game day score notifications to subscribed users via SMS/Email. It leverages Amazon SNS, AWS Lambda and Python, Amazon EvenBridge and NBA APIs to provide sports fans with up-to-date game information. The project demonstrates cloud computing principles and efficient notification mechanisms.

FEATURES

-Fetches live NBA game scores using an external API.

-Sends formatted score updates to subscribers via SMS/Email using Amazon SNS.

-Scheduled automation for regular updates using Amazon EventBridge.

-Designed with security in mind, following the principle of least privilege for IAM roles.


PREREQUISITES

Free account with subscription and API Key at football-data.org

Personal AWS account with basic understanding of AWS and Python


TECHNOLOGY

-Cloud Provider: AWS

-Core Services: SNS, Lambda, EventBridge

-External API: NBA Game API (SportsData.io)

-Programming Language: Python 3.x

-IAM Security:
Least privilege policies for Lambda, SNS, and EventBridge

PROJECT STRUCTURE

game-day-notifications/

├── src/

│   ├── gd_notifications.py          # Main Lambda function code

├── policies/

│   ├── gb_sns_policy.json           # SNS publishing permissions

│   ├── gd_eventbridge_policy.json   # EventBridge to Lambda permissions

│   └── gd_lambda_policy.json        # Lambda execution role permissions

├── .gitignore

└── README.md                        # Project documentation
