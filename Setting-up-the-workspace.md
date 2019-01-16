## Install Node.js

Visit Nodejs.org current downloads page and download appropriate installation package for your platform. 
https://nodejs.org/en/download/current/
(Latest Current Version: 11.6.0 (includes npm 6.5.0-next.0))

NPM (Node Package Manager) is included with Node.js installation.

## Install Angular CLI
Run the following npm command to install Angular CLI globally.

`
npm install -g @angular/cli
`

## Install Amplify framework
Use a command shell and run the following to install Amplify framework.

``
npm install -g @aws-amplify/cli
``
## Configure Amplify framework
Follow this step to create an IAM account that will be used by the framework to setup infrastructure for your project. More than one account can be setup and managed with profiles. Run the following command and follow instructions. 

``
amplify configure
``

