# React Native Skygear CLI

A CLI for generate react native project with skygear and other common libraries setup.

## Getting Started


### Prerequisites


```
//install react native cli
$ brew install node
$ brew install watchman
$ npm install -g react-native-cli

//install cocoapods for generate .xcworkplace
$ [sudo] gem install cocoapods
```

### Installing

Install react-native-skygear package

```
$ npm install -g oursky/react-native-skygear
```

### Example
You can start init your app from our template:

```
$ react-native-skygear init <projectname>
? Enter Skygear End Point (Development) ... 
...
```

If you also init local skygear server, please ensure shutdown other docker container before run following script.
```
$ cd server
server $ make setup-development
server $ docker-compose up
```

To run rn project:

Start RN js server
```
$ npm run start
```

For iOS:

```
1. Using Xcode, open /iOS/<projectName>.xcworkspace
2. Select "<projectName> <Development | Staging | Production>" scheme
3. Press 'Run' button
```

For Android:

```
1. Using Android Studio, open /andoird
2. Install require build tools version
3. Wait for gradle sync
4. Press 'Run' button
5. (First Time) Follow this link to ensure your device can resolve correct JS bundle url
   https://facebook.github.io/react-native/docs/running-on-device.html
```