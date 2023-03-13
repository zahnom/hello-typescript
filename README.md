# hello-typescript
Simple demo to teach how to create and publish a npm package. May also be used for tests in other projects.

# How to create and publish a npm package
We're going to setup a small typescript project:
1. Start a new npm project with npm init.
2. Install typescript with `npm install --save-dev typescript`.
3. Configure the tsconfig.json
   1. Change the output dir (e.g. `"outDir": "./build"`).
   2. Enable the generation of declaration files (.d.ts).
4. Configure the files to publish.
   1. Set "files" to the output dir (e.g. `"files": [ "build/**/*" ]`).
   2. Adapt the "main" file (e.g. `"main": "build/index.js"`).
5. Add some code.
6. Setup access to the npm registry on github.
   1. Create a .npmrc file.
   2. In the package.json: Prefix the npm package name with your account name.
   3. Log into the registry with `npm login`.
7. Build the code with `tsc`.
8. Publish package with `npm publish`.
