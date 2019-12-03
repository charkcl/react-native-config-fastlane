## Development environment setup
Install Node(10.15)

`nvm install 10.15` or `brew install node`

Install watchman(4.9.0)

`brew install watchman`

Install yarn

`brew install yarn --ignore-dependencies`

Install CocoaPods: [React-Native CocoaPods](https://facebook.github.io/react-native/docs/integration-with-existing-apps#3-install-cocoapods)

`brew install cocoapods`

### iOS setup

Please refer to https://facebook.github.io/react-native/docs/getting-started

1. Install Xcode
2. Install Xcode Command Line tools `xcode-select --install`
3. Install node modules `yarn`
4. Install CocoaPods dependencies `cd ios && pod install`

## Typescript
This project is initiated with `npx --ignore-existing react-native init <project-name> --template react-native-template-typescript`

## Secrets & Environment Variables
This project uses [react-native-config](https://github.com/luggit/react-native-config) to expose config variables to your javascript code in React Native. The `.env` files are ignored by git keeping those secrets out of your repo.

#### Get started for local development:
1. Copy `.env.example` to `.env.local` or `.env`
2. Add your config variables
3. Follow instructions at [https://github.com/luggit/react-native-config#setup](https://github.com/luggit/react-native-config#setup)
4. Secrets are usually kept in `.env.secret` and should NEVER be git committed

## Fastlane
Fastlane will load config from `/config.*` file into `.env`
Secrets are to be provided in command line

+ `MYAPP_CONFIG=prod yarn fastlane:ios-ci`
+ `MYAPP_KEYSTORE_PASSWORD=xxxxx MYAPP_CONFIG=prod yarn fastlane:android-ci`
