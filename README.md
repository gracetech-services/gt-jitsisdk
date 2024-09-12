# GraceTech Jitsi React Native SDK

## Instructions

### Create a new version of the SDK
1. Clone GraceTech jitsi-meet repo and this repo
2. Navigate to `react-native-sdk` directory in GraceTech jitsi-meet repo
3. (Optional) Run `git switch <branch name>` to switch to the desired branch in the jitsi-meet repo from which to create the new version
4. Update version in react-native-sdk `package.json` if not updated already
5. Run `npm pack --pack-destination <path to this repo>/packages/`
6. Rename the created `.tgz` file if desired and commit the file to GitHub

### Use new version of SDK in app
1. Copy raw GitHub link to the desired `.tgz` file. Make sure the link references the file from a specific commit and does not reference a branch. For example, a good link would be `https://github.com/gracetech-services/gt-jitsisdk/raw/314835fb95090505b4c24d422634eb85b988a086/packages/jitsi-react-native-sdk-0.0.0.tgz`
2. Update `@jitsi/react-native-sdk` dependency in `package.json` with the link to the `.tgz` file
