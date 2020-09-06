cat <<END > ~/.aws/config
[default]
region=ap-southeast-1
END


npx create-react-app workingDirectory
cd workingDirectory
npm start
cancel

git add .
git commit -m “install_react”
git branch -M master
git remote add origin https://github.com/piyapoonsawat/tbxFrontEnd.git
git push origin master
SEE changes in Git

git add README.md
git branch -M master
git remote add origin https://github.com/piyapoonsawat/tbxFrontEnd.git
git commit -m “install_react”
git push origin master

sudo apt-get install -y nodejs

npm install -g npm
npm install -g @aws-amplify/cli (get 4.27.3)->update to 4.28.1->4.29.0

no need "amplify configure"as already set ~/.aws/config


Goto Amplify console,
Connect to Git
User: piyapoonsawat@yahoo.com
Pass: git1q2w#E$R

Working with git
Sample of Command
// create a new repository
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/piyapoonsawat/tbxReactBackend.git
git push -u origin master

// push an existing repository
git remote add origin https://github.com/piyapoonsawat/tbxReactBackend.git
git branch -M master
git push -u origin master

//Update
git add .
git commit -m “Rev1”
git push origin master

// from tutorial 
git init
git remote add origin git@github.com:username/reponame.git
git add .
git commit -m “initial commit”
git push origin master

amplify init (use AWS profile and select "default" profile)

check amplify dashboard to see the project

amplify add auth (select without social, using email and phone)

Facebook setup: by getting Domain in Cognito,
(1) setup in "Settings -> Basic Information"
(2) in "Facebook Login -> Settings", A valid OAuth redirect URI looks like
"https://tbxbackend9314f854.auth.ap-southeast-1.amazoncognito.com/oauth2/idpresponse"
782963109145090
864e588cceadab268e9b5f95a4bad94d
email,public_profile


Google setup: by getting Domain in Cognito,
(1) create Credential -> Oauth2
(2) in original "https://tbxbackend9314f854.auth.ap-southeast-1.amazoncognito.com"
(3) in redirect "/oauth2/idpresponse"
83368141490-ei2icl3iaeq4vhvtdn6rcjuq6doq9him.apps.googleusercontent.com
AsIwOX52jKH3t3qYukavSDzF
profile email openid

 Do you want to use the default authentication and security configuration? Default configuration with Social Provider (Federation)
 How do you want users to be able to sign in? Email
 Do you want to configure advanced settings? Yes, I want to make some additional changes.
 What attributes are required for signing up? Birthdate (This attribute is not supported by Login With Amazon.), Email, Gender (This attribute
 is not supported by Login With Amazon.), Name
 Do you want to enable any of the following capabilities? 
 What domain name prefix do you want to use? tbxbackend5c4c1752-5c4c1752
 Enter your redirect signin URI: https://www.makeyourq.com/
? Do you want to add another redirect signin URI No
 Enter your redirect signout URI: https://www.makeyourq.com/
? Do you want to add another redirect signout URI No
 Select the social providers you want to configure for your user pool: Facebook, Google
 Enter your Facebook App ID for your OAuth flow:  782963109145090
 Enter your Facebook App Secret for your OAuth flow:  864e588cceadab268e9b5f95a4bad94d
 Enter your Google Web Client ID for your OAuth flow:  83368141490-ei2icl3iaeq4vhvtdn6rcjuq6doq9him.apps.googleusercontent.com
 Enter your Google Web Client Secret for your OAuth flow:  AsIwOX52jKH3t3qYukavSDzF


amplify add api 
amplify add storage


npm install aws-amplify @aws-amplify/ui-react

src/index.js
import Amplify from 'aws-amplify';
import config from './aws-exports';
Amplify.configure(config);




