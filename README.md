cat <<END > ~/.aws/config
[default]
region=ap-southeast-1
END

#Option
sudo apt-get install -y nodejs
npm install -g npm

npx create-react-app workingDirectory
cd workingDirectory
npm start
cancel

git add .
git commit -m install_react
git branch -M master
git remote add origin https://github.com/piyapoonsawat/tbxFrontEnd.git
git push origin master
SEE changes in Git

no need "amplify configure"as already set ~/.aws/config

After setting Amplify project in tbxBackend
Goto Amplify console,
Connect to Git
User: piyapoonsawat@yahoo.com
Pass: git1q2w#E$R

npm install aws-amplify @aws-amplify/ui-react

src/index.js
import Amplify from 'aws-amplify';
import config from './aws-exports';
Amplify.configure(config);




