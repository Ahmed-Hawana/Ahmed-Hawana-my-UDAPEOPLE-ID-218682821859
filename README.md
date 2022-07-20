## Author
Ahmed Hawana
Account ID: 2186-8282-1859
Federated user: voclabs/user1907529=11135712126

## UDAPEOPLE
This is a project to develop the UdaPeople product, a revolutionary concept in Human Resources which promises to help small businesses care better for their most valuable resource: their people.

## Section 1 - 
      Explain the Fundamentals and Benefits of CI/CD 
          to Achieve, Build, and Deploy Automation for Cloud-Based Software Products.

          - In the root Folder
                * presentation.pdf
                * Diagram of CI/CD Pipeline we will be building. (UdaPeople Pipeline.png) and (UdaPeople Pipeline.drawio)

## Section 2 - 
    # Geting Started:
      1- Building Frontend and Backend.
      2- Unit Test Phase.
      3- Analysis and vulnerability scan.
      4- Email Alert Settings.
    # Local Deployment:
      1- Docker and Postgres db added locally.
      2- Backend node dependancies.
      3- Frontend node dependancies.
      4- set enviromental variables.
      5- Run DB migration.
      6- lunch in development mode.
      7- build applications on production backend and frontend.
    # Starting with AWS:
      1- create EC2 keypair "udacity"
      2- create IAM user "udapeople-circleci-runner".
      3- Add postgres SQL DB in AWS RDS which is public.
      4- Cloudfront destribution
            a- choose random string "a01a01", create public S3 bucket "udapeople-random string"
            b- run circleci/files/cloudfront.yml
      5- Circleci 
            a- ADD the EC2 Key pair.
            b- Setup environment variables.
      6- Deploy Infrastructure
            a- Install AWSCLI
            b- Ensure Backend Infrastructure 
            c- Ensure frontend Infrastructure
            d- add ip address to Ansible Inventory
            e- persist inventory file to workspace
            f- add rollback command in case of failure:
                  - Delete backend stack
                  - Empty frontend bucket
                  - Delete front end stack
      7- Configure Infrastructure
            a- Configure server Ansible playbook
            b- Configure server Ansible task
            c- Update Prometheus Node Exporter to latest version.
            d- complete job steps in config.yml
      8- Migration
            a- create account on kvdb.io
            b- Store kvdb bucket name on CircleCi
            c- run migration script on Nodejs
            d- add revert migration
      9- Deployment at production
            a- Deploy backend production app to EC2 instance
            b- Deploy frontend production static files to S3 bucket
      10- Smoketest
            a- run on backend
            b- run on frontend
      11- Promotion and cleanup
            a- store last workflow ID exported by initial stack to be used later.
            b- Update initial stack cloudfront to point to the latest frontend bucket
            c- after successful update, delete all old stacks.


# ScreenShots
    On the root Folder my screenshots folder contains:-
      - screenshots in JPG, named using the screenshot number listed as follow:
          1. Job failed because of compile errors. [SCREENSHOT01].
          2. Job failed because of unit tests. [SCREENSHOT02].
              for the backend and [SCREENSHOT02-2] for the frontend.
          3. Job that failed because of vulnerable packages. [SCREENSHOT03]
              for the backend and [SCREENSHOT03-2] for the frontend.
          4. An alert from one of my failed builds. [SCREENSHOT04]          
          5. Appropriate job failure for infrastructure creation. [SCREENSHOT05] 
          6. Appropriate job failure for the smoke test job. [SCREENSHOT06]
          7. Successful rollback after a failed smoke test. [SCREENSHOT07]
          8. Successful promotion job. [SCREENSHOT08]
          
          9.URLS 
                  a- Public Url to GitHub repository [URL01_SCREENSHOT]
                  b- Public URL for your S3 Bucket [URL02_SCREENSHOT]
                  c- front-end application in CloudFront [URL03_SCREENSHOT], [URL03-2_SCREENSHOT]
                  d- Public URLs to deployed application back-end in EC2 [URL04_SCREENSHOT]
                  e- Public URL to your Prometheus Server [URL05_SCREENSHOT]
          10. 



### Built With

- [Circle CI](www.circleci.com) - Cloud-based CI/CD service
- [Amazon AWS](https://aws.amazon.com/) - Cloud services
- [AWS CLI](https://aws.amazon.com/cli/) - Command-line tool for AWS
- [CloudFormation](https://aws.amazon.com/cloudformation/) - Infrastrcuture as code
- [Ansible](https://www.ansible.com/) - Configuration management tool
- [Prometheus](https://prometheus.io/) - Monitoring tool



###### #############################################################################3
###### ###############################################################################
###### ****************************************************************************************
######
#  We are archiving this repository because we do not want learners to push personal development to the current repository. If you have any issues or suggestions to make, feel free to:
    - Utilize the https://knowledge.udacity.com/ forum to seek help on content-specific issues.
    - [Submit a support ticket](https://udacity.zendesk.com/hc/en-us/requests/new) along with the link to your forked repository. 
    - If you are an enterprise learner, please [Submit a support ticket here](https://udacityenterprise.zendesk.com/hc/en-us/requests/new?ticket_form_id=360000279131)

## Give your Application Auto-Deploy Superpowers

In this project, you will prove your mastery of the following learning objectives:

- Explain the fundamentals and benefits of CI/CD to achieve, build, and deploy automation for cloud-based software products.
- Utilize Deployment Strategies to design and build CI/CD pipelines that support Continuous Delivery processes.
- Utilize a configuration management tool to accomplish deployment to cloud-based servers.
- Surface critical server errors for diagnosis using centralized structured logging.

![Diagram of CI/CD Pipeline we will be building.](udapeople.png)

### Instructions

* [Selling CI/CD](instructions/0-selling-cicd.md)
* [Getting Started](instructions/1-getting-started.md)
* [Deploying Working, Trustworthy Software](instructions/2-deploying-trustworthy-code.md)
* [Configuration Management](instructions/3-configuration-management.md)
* [Turn Errors into Sirens](instructions/4-turn-errors-into-sirens.md)

### Project Submission

For your submission, please submit the following:

- A text file named `urls.txt` including:
  1. Public Url to GitHub repository (not private) [URL01]
  1. Public URL for your S3 Bucket (aka, your green candidate front-end) [URL02]
  1. Public URL for your CloudFront distribution (aka, your blue production front-end) [URL03]
  1. Public URLs to deployed application back-end in EC2 [URL04]
  1. Public URL to your Prometheus Server [URL05]

- Your screenshots in JPG or PNG format, named using the screenshot number listed in the instructions. These screenshots should be included in your code repository in the root folder.
  1. Job failed because of compile errors. [SCREENSHOT01]
  1. Job failed because of unit tests. [SCREENSHOT02]
  1. Job that failed because of vulnerable packages. [SCREENSHOT03]
  1. An alert from one of your failed builds. [SCREENSHOT04]
  1. Appropriate job failure for infrastructure creation. [SCREENSHOT05]
  1. Appropriate job failure for the smoke test job. [SCREENSHOT06]
  1. Successful rollback after a failed smoke test. [SCREENSHOT07]  
  1. Successful promotion job. [SCREENSHOT08]
  1. Successful cleanup job. [SCREENSHOT09]
  1. Only deploy on pushed to `master` branch. [SCREENSHOT10]
  1. Provide a screenshot of a graph of your EC2 instance including available memory, available disk space, and CPU usage. [SCREENSHOT11]
  1. Provide a screenshot of an alert that was sent by Prometheus. [SCREENSHOT12]

- Your presentation should be in PDF format named "presentation.pdf" and should be included in your code repository root folder. 

Before you submit your project, please check your work against the project rubric. If you haven’t satisfied each criterion in the rubric, then revise your work so that you have met all the requirements. 

###### *************************************************************************
###### ##########################################################################

### License

[License](LICENSE.md)


###### ########################################################################3
###### ########################################################################