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
