# How I Learned To Stop Worrying And Love The Failed Build

## Me and what I do
[PIC OF ME]


# History of release times
1994-1998 - GPT - 2 year release cycle
1998-2002 - AIT - < 1 year
2002-2008 - 1 month
2008-2012 - 2 week (SCRUM)
NOW - many a day

[GRAPH]

# Agile Manifesto
"Our highest priority is to satisfy the customer through early and continuous delivery of valuable software."
Agile Manifesto 2001 AD

# Jez and David Publish book
READ BOOK


## Continuous Deployment 

Steps to CD
- Deployment must be repeatable and reliable
- No Manual Steps
- If it hurts do it more often
- Keep everything in source control
- It's not done until it's released
- Measure, measure, measure
- Everybody is responsible for the release process
- Continuously improve

Best Practices:
- Build once
- Consistent deployment to all evironments - Use the same mechanism to deploy to all environments
- Smoke tests
- Failure stops the pipeline
- Don't patch





## Resources:
Agile Manifesto:
http://agilemanifesto.org/principles.html

Continuous Delivery: Reliable Software Releases through Build, Test, and Deployment Automation
Jez Humble and David Farley
http://www.amazon.co.uk/dp/B003YMNVC0



Our highest priority is to satisfy the customer
through early and continuous delivery
of valuable software.












##############################################
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

- Who does continuous deployment?
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

