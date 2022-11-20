We  just configure our custom command inside the package.json file under the scripts section.

say  we have the following:
"myCode" :"npx cypress open"

Then, we can run this command on terminal or on Jenkins using npm run myCode

### On jenkins when project is on github
Create a job
Under SCM, select git and provide the url to the project and the credentials and specify the branch
Proceed to Build step section, select Execute shell and run the custom command you would actually run on terminal `npm run myCode`

Save the project and build the job. Proceed to view the output on console

#### On jenkins when project is on local machine
Create a job
Under genral section, select use custom wprkspace and provide the path to the project on your machine `/Users/mac/Documents/Cypress/Cypress_Jenkins` 
Proceed to Build step section, select Execute shell and run the custom command you would actually run on terminal `npm run myCode`

Save the project and build the job. Proceed to view the output on console
