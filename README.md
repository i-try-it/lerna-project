As a developer i did not want to setup lerna globaly

1. npm init
2. npm i --save-dev lerna
3. add script ``"lerna-init": "node ./node_modules/lerna/bin/lerna.js init"``

    ``lerna init`` - Create a new lerna repo or upgrade an existing repo to the current version of Lerna.
4. run npm run lerna-init


# There are 2 modes
## fixed/locked (default)
Fixed mode Lerna projects operate on a single version line. 
The version is kept in the lerna.json file at the root of your project under the version key.

 ``lerna publish`` -  if a module has been updated since the last time a release was made, it will be updated to the new version you're releasing. This means that you only publish a new version of a package when you need to.
## independent (--independent)
