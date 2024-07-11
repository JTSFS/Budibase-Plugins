# Basic Steps
- Fork existing plugin from Github
- Change up the code however you want
- Navigate to import plugin, upload file, upload Tarball file

## Building the plugin
- Install Node.js
- Install npm
- Install Homebrew
- Install python@3.10
- Navigate to the Project Directory
- npm run build

## Notes
- There may be pieces of the plugin that need to be updated/removed and readded
  - EX: npm install --save-dev rollup
  - EX: rm -rf node_modules
  - EX: npm install rollup-plugin-copy2 --save-dev
  - EX: rm -rf node_modules package-lock.json
- If the plugin packages have the rollup, create tarball, etc... Those steps can be skipped as they are done automatically.
- stateStore houses the states, can be accessed by the component
-   stateStore is pulled in by const { styleable, Provider, API, builderStore, stateStore } = getContext("sdk");
-   States are pulled in by stateStore.subscribe($state => { brokerId = $state.broker_id });
