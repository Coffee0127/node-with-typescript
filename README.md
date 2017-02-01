# Visual Studio Code: Node.js with TypeScript and Debugging
### Setup
1. [NodeJS](http://www.nodejs.org/)
2. TypeScript  
type `npm install typescript -g` in the terminal
3. [Visual Studio Code](http://code.visualstudio.com/)

### Steps
1. A new project  
type `npm init -y`
2. Install Node.js declaration files  
type `npm install @types/node --save-dev`
3. TypeScript compiler configuration  
create `tsconfig.json` file
    ```json
    {
      "compilerOptions": {
        "module": "commonjs",
        "sourceMap": true,
        "watch": true
      }
    }
    ```

### Reference
* [Visual Studio Code: Node.js with TypeScript and Debugging](http://www.cross-platform-blog.com/tools/nodejs/typescript/visual-studio-code-nodejs-with-typescript-and-debugging/)
