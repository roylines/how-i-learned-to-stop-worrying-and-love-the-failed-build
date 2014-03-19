# How I Learned To Stop Worrying And Love The Failed Build

## Me and what I do
[PIC OF ME]


# History of release times
In my lifetime releases have sped up. 
In 1996 the company I worked for had a release time of 2 years. 
It was a long drawn out waterfall process. Manual builds, manual tests, sign-off.
By 2000 we were down to yearly releases. Still waterfall, still manual builds and large integration points.
Agile manifesto was published in 2001, and by 2003 release times were down to 1 month, then every 2 weeks through 2009 to 2012

- releases speeded up.
- waterfall -> agile

# Agile Manifesto
"Our highest priority is to satisfy the customer through early and continuous delivery of valuable software."
Agile Manifesto 2001 AD

The two week release cycle was largely an artifact of scrum and two week iterations, and frankly this felt pretty good. 
By now CI servers were an essential part of the process and Id got into the habit of measuring things: code quality and complexity, coverage.

# Jez and David Publish book
In 2010 Jez Humble and David Farley of Thoughtworks published : Continuous Delivery

Firstly the book is called Continuous Delivery, but actually the most enlightening part for me is the concept of Continuous Deployment.
"Software release can - and should - be a low-risk, frequent, cheap, rapid and predictable process"

Continuous deployment is the logical extension of Continuous Integration covering more than just software development
Reduce cycle time: the time it takes from deciding to make a change to having it available for users.

"Find ways to deliver high-quality, valuable software in an efficient, fast and reliable manner"
- low cycle time
- high quality

## Continuous Deployment 
What are the steps to continuous deployment

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

 Key to it all is the deployment pipeline




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

