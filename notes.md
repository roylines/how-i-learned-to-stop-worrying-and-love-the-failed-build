# Notes

## Images?
- ascent of man
- sugar
- scooby doo

## Introduction
- Me
- C -> C++ -> C# -> JS
- In the early days things just took time - largely due to Waterfall processes
  - Long development periods followed by long testing periods
- Things got quicker - SCRUM and sprints
  - Shorter and shorter release cycles - still slowed down by QA Testing.

- Five Steps - Eric Reiss
  - Continuous Integration Server
  - Source Control Commit Check
  - Deployment Script
  - Alerting
  - Root Cause Analysis (5 Whys)

- Then I read this book.
  - read the book

- Who does continuos deployment?
 - http://www.quora.com/Continuous-Deployment/Which-companies-are-doing-Continuous-Delivery-Continous-Deployment-really-well
 - IMVU, GitHub, Etsy, Facebook

 - http://radar.oreilly.com/2009/03/continuous-deployment-5-eas.html

- What do we do - node servers
  - CI - go, tests are mocha, casperjs. enforce code coverage etc...
  - GitHub pre-commit hooks - check tests run ok and that the build is green
  - Auto deployment to EC2 - ec2-each
  - Smoke tests: UI using casperjs and web services using mocha
  - Loggly, New Relic and CloudWatch to monitor the production system.
  - Root cause analysis - always asking why we didnt trap it throught the system

- Did we fire the testers?
  - No. Different objective - now they dont stop releases - they test production for things that have slipped through.
