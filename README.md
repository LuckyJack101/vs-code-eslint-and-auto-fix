# Setting up eslint and auto fix for react

## Links
- https://www.youtube.com/watch?v=SydnKbGc7W8
- https://www.youtube.com/watch?v=YIvjKId9m2c
- https://www.npmjs.com/package/eslint-config-airbnb

## How to setup

### 1. Install these dependencies
- Base
  - npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier
- AirBnB
  - npm i -D eslint eslint-plugin-import eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-jsx-a11y
 
### 2. Create the .eslintrc file
- You can use the file from this project
- Add it to the root of your project

### 3. Update your vs code settings json
- To enable autofix you need to add these to your settings json file
```json
"editor.formatOnSave": true,
    "[javascript]": {
        "editor.formatOnSave": false
    },
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
    },
    "eslint.alwaysShowStatus": true,
```

## How to use
- Open/create a .js file and see linting is shown and auto-fix is working on save

## Notes

- npx install-peerdeps --dev eslint-config-airbnb
  - This command does not work on a create-react-app
  - Instead use the suggestion mentioned above
