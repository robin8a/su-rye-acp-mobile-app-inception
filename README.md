# su-rye-acp-mobile-app-inception
# References
- [Getting started](https://docs.amplify.aws/start/q/integration/react-native)
- [The fastest way to build an app](https://expo.io/)
- [Create a new React Native app](https://reactnative.dev/docs/environment-setup)

# AWS Amplify Setup

Sign in to your AWS administrator account:
https://console.aws.amazon.com/
Press Enter to continue

Specify the AWS Region
? region:  us-east-1
Specify the username of the new IAM user:
? user name:  su-amplify
Complete the user creation using the AWS console
https://console.aws.amazon.com/iam/home?region=undefined#/users$new?step=final&accessKey&userNames=su-amplify&permissionType=policies&policies=arn:aws:iam::aws:policy%2FAdministratorAccess
Press Enter to continue

Enter the access key of the newly created user:
? accessKeyId:  AKIASSMSUP**********
? secretAccessKey:  c+SyFi3s+A8N7WwBLJ7+********************
This would update/create the AWS Profile in your local machine
? Profile Name:  su-rye-acp


# Creating expo client

```sh
npm install -g expo-cli  

#install cocoa with sudo
sudo expo init testBorrar

expo init suRyeAcpMobileApp

Downloaded and extracted project files.
✔ Installed JavaScript dependencies.
⠹ CocoaPods CLI not found in your PATH, installing it now.Your password might be needed to install CocoaPods CLI: https://guides.cocoapods.org/using/getting-started.html#installation
⚠️  Unable to install the CocoaPods CLI. Continuing with initializing the project, you can install CocoaPods afterwards.

✅ Your project is ready!

To run your project, navigate to the directory and run one of the following yarn commands.

- cd suRyeAcpMobileApp
- yarn android
- yarn ios
- yarn web

💡 You can also open up the projects in the ios and android directories with their respective IDEs.
🚀 expo-updates (​https://github.com/expo/expo/blob/master/packages/expo-updates/README.md​) has been installed in your project. Before you do a release build, you'll need to configure a few values in Expo.plist and AndroidManifest.xml in order for updates to work.

⚠️  Before running your app on iOS, make sure you have CocoaPods installed and initialize the project:


```

# Git 
```sh

git remote add origin ssh://git-codecommit.us-east-1.amazonaws.com/v1/repos/suRyeAcpMobileApp
git remote -v

# origin  ssh://git-codecommit.us-east-1.amazonaws.com/v1/repos/suRyeAcpMobileApp (fetch)
# origin  ssh://git-codecommit.us-east-1.amazonaws.com/v1/repos/suRyeAcpMobileApp (push)

git push --set-upstream origin master


```

# AWS Profile

```sh
less ~/.aws/config


# [profile su-rye-acp]
# region=us-east-1

# To use a named profile for multiple commands, you can avoid specifying the profile in every command by setting the AWS_PROFILE environment variable at the command line.

## Linux or macOS

export AWS_PROFILE=su-rye-acp

```


# Testing

```sh
cd suRyeAcpMobileApp
npm start # you can also use: expo start
expo start

```