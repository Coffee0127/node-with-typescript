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

4. [Start the TypeScript compiler with Visual Studio Code](http://www.cross-platform-blog.com/tools/nodejs/typescript/visual-studio-code-nodejs-with-typescript-and-debugging/#start-the-typescript-compiler-with-visual-studio-code)
5. [Debug the Node.js application](http://www.cross-platform-blog.com/tools/nodejs/typescript/visual-studio-code-nodejs-with-typescript-and-debugging#debug-the-nodejs-application)  
modified default `launch.json`, add the following configuration to enable sourceMap  
For more detail please see the [launch.json](https://github.com/Coffee0127/node-with-typescript/blob/master/.vscode/launch.json)

    ```json
      "sourceMaps": true,
      "outFiles": [ "${workspaceRoot}/dist/**/*.js" ]
    ```

### Reference
* [Visual Studio Code: Node.js with TypeScript and Debugging](http://www.cross-platform-blog.com/tools/nodejs/typescript/visual-studio-code-nodejs-with-typescript-and-debugging/)
* [tsconfig.json](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html)
* [从JavaScript迁移到TypeScript](https://zhongsp.gitbooks.io/typescript-handbook/content/doc/handbook/tutorials/Migrating%20from%20JavaScript.html)
* [Unable to debug TypeScript project after VSCode update.](https://github.com/Microsoft/vscode/issues/7745#issuecomment-254924638)
