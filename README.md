# Prepare-Angular-Project

Prepare the project for development. We'll install and configure: Prettier & Stylelint-code
to be nice, esLint-code to be clean, jest for testing code faster, huskey-to automate the
linting and formatting process before sending the changes to the remote repository.

All extensions will have their own branch with changes before merging into the main
branch.

1.Stylelint - https://stylelint.io/ - We set the configuration and the rules depending on the documentation. linting is set only for scss files, if you want to add css files, add css in script in package.json file - "stylelint": "stylelint \"src/\*\*/\*.{css,scss}\" --fix --cache",
Branch name is Stylelint
