# bass-mobile-starter
Boilerplate starter template for a hybrid Ionic2 mobile app using firebase as a hosting and database provider but using Auth0 

We are using the Ionic framework to set up the  framework of our app first 
INSERT IONIC COMMANDS


##Create GitHub Account
Create github account at [GitHub](https://github.com)

##Create Firebase Account
Create a firebase account with your google account for our back end database and hosting at [Firebase](https://firebase.google.com/)

*Navigate to the [Firebase Console](https://console.firebase.google.com/) where you will manage your firebase application.

*Click 'Create new project'
**Select the name as 'bass-demo' and click continue.
*Find the Hosting card and click get started.
Click get started again.


Use the npm command in the project root directory:  (You can do this in Visual studio code by using the ` shortcut)
$ npm install -g firebase-tools

We are using npm to install firebase tools using the global tag which does not add the package to your package.json.

Click continue while that installs.

Next we will login with;
$ firebase login
Enter N to not share CLI data collection
A browser will pop up to link the Command Line tool to your firebase account. 

Now in your .firebaserc file, replace the default value with the name of the firebase project you created.
"{
  "projects": {
    "default": "bass-demo"
  }
}"
We are using bass-demo for this template.

Next run the command 
$ firebase init

This will initalize our firebase configuration files (firebase.json and .firebaserc) to configure our firebase application. Use the arrow keys and space bar to de-select the functions setup option. We only need hosting and database features.

Select the name of the firebase project to associate as the default, 'bass-demo'.
Use the Default databaserules json file by hitting enter.

Use 'platforms/browser/www' for the public directory folder. This is where our Ionic CLI will deploy our browser code.

Select y to configure the app as a single-page app.

Now lets test our configuration out by running 
firebase deploy
We shouuld see a success messare on the HOSTING URL link that the console displays. Since our platforms/browser/www directory was empty Firebase initalized a test index.html page for us that will be rewritten later.


##Create Auth0 Account
Create an Auth0 account for our authentication service at [Auth0](https://auth0.com/) 

##Create CodeShip Account
Create a Codeship account to automatically deploy our latest build when it passes our automated tests at [CodeShip](https://codeship.com)
