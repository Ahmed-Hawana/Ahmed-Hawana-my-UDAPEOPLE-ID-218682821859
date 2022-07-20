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
      12- Prometheus


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
          9. Successful cleanup job. [SCREENSHOT09]
          10. Only deploy on pushed to `master` branch. [SCREENSHOT10]
          11. Provide a screenshot of a graph of your EC2 instance including available memory, available disk space, and CPU usage. [SCREENSHOT11]
          12. Provide a screenshot of an alert that was sent by Prometheus. [SCREENSHOT12]
          13. URLS 
                  a- Public Url to GitHub repository [URL01_SCREENSHOT]
                  b- Public URL for your S3 Bucket [URL02_SCREENSHOT]
                  c- front-end application in CloudFront [URL03_SCREENSHOT], [URL03-2_SCREENSHOT]
                  d- Public URLs to deployed application back-end in EC2 [URL04_SCREENSHOT]
                  e- Public URL to your Prometheus Server [URL05_SCREENSHOT]
          
### Built With

- [Circle CI](www.circleci.com) - Cloud-based CI/CD service
- [Amazon AWS](https://aws.amazon.com/) - Cloud services
- [AWS CLI](https://aws.amazon.com/cli/) - Command-line tool for AWS
- [CloudFormation](https://aws.amazon.com/cloudformation/) - Infrastrcuture as code
- [Ansible](https://www.ansible.com/) - Configuration management tool
- [Prometheus](https://prometheus.io/) - Monitoring tool

### License

[License](LICENSE.md)


###### ########################################################################3
###### ########################################################################