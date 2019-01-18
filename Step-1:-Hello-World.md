In this section, we will setup the workspace and create all the boiler plate template needed for the workshop.

## Create Workspace
Create a workspace folder called 'ws' (or any name of your choice) and go to that folder.

`mkdir ws`

`cd ws`

## Create Angular Boilerplate
While in the workspace folder, create new Angular application boiler plate using Angular CLI. In this example, will use frontend as the name of the Angular app.

`
ng new frontend --routing
`

This may take a minute or two, depending on the internet connection speed as it will create boiler plate template and install all dependencies.

Once completed, go to the frontend folder and serve to verify everything is working properly. 

`cd frontend`

`ng serve --o`

This will open your default browser and display the default page at http://localhost:4200. This ensures that Angular framework is fully setup and working without any issues.

## Initialize Amplify
Now we will initialize Amplify framework in the root folder named 'ws'. **Do not do this in frontend folder.**

`cd ..`

`amplify init`

Follow prompts to finish the rest of the steps to finish the process. Here are sample responses:
* ? Enter a name for the project awsslsws
* ? Choose your default editor: Visual Studio Code
* ? Choose the type of app that you're building javascript
* Please tell us about your project
* ? What javascript framework are you using angular
* ? Source Directory Path:  frontend/src
* ? Distribution Directory Path: frontend/dist/frontend
* ? Build Command: ng build 
* ? Start Command: ng serve --o

## Setup Hosting
Now setup Hosting on AWS. Amplify will orchestrate to setup S3 with CloudFormation.

`amplify hosting add`

Follow prompts to finish the activity. Choose 'DEV' option instead of 'PROD' option. Leave the rest to defaults.

## Publish the application
Its now go live time! Let's publish it to see if everything is ready

`cd frontend`

`amplify publish`

When prompted to confirm, type 'y' to go ahead. On first publish, this may take a few minutes. But once completed, you should see the CloudFront URL where your application is available for users. 

