# DevhubWorkshop
Here is a list of all actions in github: 
https://github.com/marketplace?type=actions


Create an action with the yml file at .github/workflows/ci-pipeline.yml
This file already has the basic steps (install .net, package restore ect)
 
Code quality and testing
1. Run the tests

2. Implement linting
   You can use JetBrains.ReSharper.GlobalTools
   Output the insepction to a jsonfile
   In a seperate action, use the analyzation script found under .github/scripts to analyze the findings from the inspection

3. Static code analysis
   Log into 1password. Find the SonarQube item. Click on website url and login with the 1password credentials.
   Create a new project with your own credentials.
   Follow the guide provided in SonarQube
   Hint: Sonar token can be created here: User > My Account > Security

Dependencies
Security scanning 
1. Implement Git leaks
   You can use github's own action for this: https://github.com/marketplace/actions/gitleaks
   If you find any vulnerabilties in the ShoppingCart application - fix them!
   
2. Implement Zap Scan
   Google something like "github actions zap scanner".
   There should be a couple of different free to use zap scanners.

   
