# Postman API Automation Integration with Github Actions #

This repository is a demonstration for POC for integrating Postman with github actions. The tests are written in Postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra.
Github Actions will trigger the project execution on every push to the main branch. You can also execute the project manually using workflow_dispatch. The project runs on scheduled time with the help of cron job.

The HTML report is archieved and kept in the artifact section for the team to download it. Along with that they can view the report directly from the github page : https://ojhaankit116.github.io/Phoenix-Inwarranty-Flow/
The Latest Report is mailed to the team members using GMAIL SMTP.

## About Me ##
Hi My Name is Ankit Ojha. I have 4 years of experience in Manual and Automation Testing. My skillset includes UI Automation with Selenium Webdriver, Cypress, Playwright and API Testing I use Rest Assured and Postman. You can connect with me over : www.linkedin.com/in/ankit-ojha-713a5012b 

## Testing Coverage ##
1. Happy Flow Testing
2. Negative Testing and Edge Case Testing
3. Token Testing
4. Data Driven Testing with csv
5. Schema Validation
6. Secrets Management with Github secrets

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

## HTML Report ##
The Report will be created in the newman folder
![Postman Report](https://github.com/ojhaankit116/Phoenix-Inwarranty-Flow/blob/static-content/newman-report.png)


## Project Structure ##
```
Phoenix Inwarranty flow
├─ Inwarranty-flow Collection.postman_collection.json  # Collection file
├─ QA.postman_environment.json # Environment file
└─ testdata.csv # TestData file

```

## How to run the project ##
You can run the project on your local system:
1. Clone the Project on Local System: https://github.com/ojhaankit116/Phoenix-Inwarranty-Flow
2. Install Nodejs and NPM from: https://nodejs.org/en
3. Install Newman: ``` npm install -g newman ```
4. Install newman-html-reporter: ``` npm install -g newman-reporter-htmlextra ```
5. Run the newman command:
```
              newman run 'Inwarranty-flow Collection.postman_collection.json' \
              -e QA.postman_environment.json \
              -d testdata.csv \
              -r cli,htmlextra \
              --reporter-htmlextra-export ./newman/index.html
```


