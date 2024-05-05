## how to setup a new Typescript express project

1. npm init -y
2. npm i -D typescript
3. npx tsc --init, npm i concurrently


4. add the following scripts in package.json
 {
    "build": "npx tsc",
  "watch": "npx tsc -w",
  "start": "npx nodemon dist/index.js",
  "dev": "concurrently -k \"npm run watch\" \"npm run start\""
  }

5. npm run dev  
