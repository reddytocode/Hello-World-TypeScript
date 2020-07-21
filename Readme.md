# Hello World in TypeScript

- Create a new folder

```bash
mkdir hello-world
cd hello-world
```

- Initialize a new npm project

```bash
npm init
```

- install TSC, TSLint and type declarations for nodeJS

```bash
npm install --save-dev typescript tslint @types/node
```

- Create tsconfig.json

Create a file called **tsconfig.json** and place the following code inside

```json
{
  "compilerOptions": {
    "lib": ["es2015"],
    "module": "commonjs",
    "outDir": "dist",
    "sourceMap": true,
    "strict": true,
    "target": "es2015"
  },
  "include": ["src"]
}
```

- Generate the TSLint default configuration

Just run the command

```bash
./node_modules/.bin/tslint --init
```

## Start the configuration of the files

- Create **src** folder

```bash
mkdir src
cd src
```

So, the structure of the files will llook like this:

```
hello-world/
├──node_modules/
├──src/
│ └──index.ts
├──package.json
├──tsconfig.json
└──tslint.json
```

- Write inside **index.ts** a console log statement

```TS
console.log("Hello World")
```

## Compile and Run

- Copmile the TypeScript code

```bash
./node_modules/.bin/tsc
```

- Run your code with NodeJS

```bash
node ./dist/index.js
```

That's all... Happy coding! :D
