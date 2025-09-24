# Postman API Automation Integration with Github Actions #

This repository is a demonstration for POC for integrating Postman with github actions. The tests are written in Postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra.
Github Actions will trigger the project execution on every push to the main branch. You can also execute the project manually using workflow_dispatch. The project runs on scheduled time with the help of cron job.

The HTML report is archieved and kept in the artifact section for the team to download it. Along with that they can view the report directly from the github page : https://ojhaankit116.github.io/Phoenix-Inwarranty-Flow/
The Latest Report is mailed to the team members using GMAIL SMTP.


## Tech Stack ##
1. Postman
2. Nodejs 22v
3. Newman
4. Newman-Reporter-Htmlextra
5. Github Actions
6. Gmail SMTP
7. Github Pages
8. CSV for Data Driven Testing
9. AWS-EC2 instance for Self hosted github runner

## Github Pages ##
You can directly view the latest test report of the Postman Test at the Github Page Link: https://ojhaankit116.github.io/Phoenix-Inwarranty-Flow/

## How to run the project ##
You can run the project on your local system:
1. Clone the Project on Local System: https://github.com/ojhaankit116/Phoenix-Inwarranty-Flow
2. Install Nodejs and NPM from: https://nodejs.org/en
3. Install Newman: npm install -g newman
4. 
