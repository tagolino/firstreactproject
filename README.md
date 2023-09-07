# First React Project

---

First React JS project. Can be use as boiler plate when starting a new React JS project.

---

##### Steps to start a new project

1. Create repository
   a. `.gitignore`
   - Select "Node"
2. Clone repository in local machine
   b. `git clone <repo URL>`
3. Change directory to new React JS project
4. Make sure Node.js is already installed in the machine
5. Run `$ npx create-react-app .`
   a. `npx` is already installed when Node.js is installed
   b. Wait until process is finished
6. Setup ESLint and Prettier formmatter
   a. [How to Setup ESLint and Prettier for Your React Apps](https://dev.to/thomaslombart/how-to-setup-eslint-and-prettier-for-your-react-apps-1n42)
   b. Add "eslintConfig" and "prettier" key in your `package.json` file.

   ```
   {
        "prettier": {
            "singleQuote": false,
            "printWidth": 100,
            "semi": true,
            "tabWidth": 2
        }
   }
   ```

   c. Or create `.eslintrc.json` and `.prettierrc.json` files.

   ```
   {
        "env": {
            "node": true,
            "browser": true,
            "es2021": true,
            "jest": true
        },
        "extends": [
            "eslint:recommended",
            "plugin:react/recommended"
        ],
        "overrides": [
        ],
        "parserOptions": {
            "ecmaVersion": "latest",
            "sourceType": "module"
        },
        "plugins": [
            "react"
        ],
        "rules": {
            "react/react-in-jsx-scope": "off",
            "react/prop-types": "off",
            "react/display-name": "off",
            "no-extra-boolean-cast": "off"
        }
   }
   ```

   ```
   {
        "singleQuote": false,
        "printWidth": 100,
        "semi": true,
        "tabWidth": 2
   }
   ```

7. Run `$ npm start`
