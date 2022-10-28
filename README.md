# Prepare-Angular-Project

Prepare the project for development. We'll install and configure: **Prettier** & **Stylelint**-code
to be nice, **esLint**-code to be clean, jest for testing code faster, **Husky**-to automate the
linting and formatting process before sending the changes to the remote repository. **commitlint** - checks if your commit messages meet the [conventional commit format](www.conventionalcommits.org)

All extensions will have their own branch with changes before merging into the main
branch.

1. Stylelint - https://stylelint.io/ - We set the configuration and the rules depending on the documentation. linting is set only for scss files, if you want to add css files, add css in script in package.json file - "stylelint": "stylelint \"src/\*\*/\*.{css,scss}\" --fix --cache".  
   Branch name is Stylelint

2. EsLint - https://eslint.org/ - We set the configuration and the rules depending on the documentation. For Angular, eslint has its own command which helps easily configure all the eslint setup that we need. - ng add @angular-eslint/schematics - If you use the VsCode IDE, set the eslint extension and it will show you problems live. If it doesn't work, restart the IDE.  
   Branch name is EsLint

3. Prettier - https://prettier.io/ - We set the configuration and the rules depending on the documentation. - npm install prettier eslint-plugin-prettier eslint-config-prettier --save-dev - This command, in addition to installing Prettier, also takes care of the installation of two packages that disable some ESLint rules to avoid conflicts with Prettier.  
   Branch name is Prettier

4. Husky - https://typicode.github.io/husky/#/ - We set the configuration and the rules depending on the documentation. we use lint-staged - https://www.npmjs.com/package/lint-staged - to run few scripts before commit.  
   Branch name is husky

5. commitlint - https://github.com/conventional-changelog/commitlint/#what-is-commitlint - With the help of Husky, we will automate the process of committing  
   Branch name is commitlint

6. Jest - https://jestjs.io/ - [configuration gide for Angular](https://medium.com/@kyjungok/setup-jest-in-angular-application-22b22609cbcd), Jest is a delightful JavaScript Testing Framework with a focus on simplicity. It's very fast and easy for us.  
   Branch name is Jest

7. Angular Material & Bootstrap - https://material.angular.io/ - https://getbootstrap.com/ - From bootstrap we'll use grid, utilities, helpers, containers. From Material we'll use components and themes  
   Branch name is Material-Bootstrap
