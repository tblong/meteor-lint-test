# Linting in Meteor
Example base Meteor project setup using VS Code and ESLint:

* [VS Code: ESLint extension](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
* [Meteor Guide: Installing and running ESLint](http://guide.meteor.com/code-style.html#eslint-installing)

# Recreating this project's setup from scratch

1. Add [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) extension to VS Code  
2. Create new meteor project: `meteor create my_project`
3. Change to new project directory: `cd my_project/`
4. Add linting modules:

    ```
    meteor npm install --save-dev babel-eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-meteor eslint-plugin-react eslint-plugin-jsx-a11y@^1.2.0 eslint-import-resolver-meteor eslint@^2.9.0
    ```

5. Install all explicit and dependent node modules: `meteor npm install`
6. Add `scripts` and `eslintConfig` settings shown in this project's `package.json` file
7. Run the linter to test code: `meteor npm run lint`
