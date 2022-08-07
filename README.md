# cypress_automation

## 📖 Overview

> * This project uses Cypress.io framework to perform end-to-end testing.
> * Cypress is a next-generation front-end test tool designed for the modern web.
> * Cypress is not subject to the same restrictions as selenium.
> * This allows you to write tests faster, easier and more reliable.

## 🔗 Useful links

> * [Docs](https://docs.cypress.io/guides/overview/why-cypress "Docs")
> * [Key Differences](https://docs.cypress.io/guides/overview/key-differences#What-you-ll-learn "Key Differences")
> * [npm vs yarn](https://docs.cypress.io/guides/getting-started/installing-cypress#What-you-ll-learn "npm vs yarn")
> * [Cypress and Page object model](https://www.cypress.io/blog/2019/01/03/stop-using-page-objects-and-start-using-app-actions/ "Cypress and Page object model")
> * [Best practices](https://docs.cypress.io/guides/references/best-practices "Best practices")

## 🧰 Prerequisite

> * Node installed
> * An IDE (visual studio recommanded)

## 🛠️ Tips

> * [Volta (recommanded)](https://docs.volta.sh/guide/getting-started "Volta (recommanded)")
> * [nvm](https://github.com/nvm-sh/nvm "nvm")
> * [WSL](https://docs.microsoft.com/fr-fr/windows/wsl/install "WSL")
>
> * If you are using a Mac and find that typing all the command `npx cypress open` is time consuming you can create an alias by running the following commands:
>
> 1. cd
> 2. `nano .zshrc` OR `vim .zshrc`
> 3. Add the following functions to your file :
>
> function cyo (){
> npx cypress open --env allure=true
> }
>
> function cyr () {
> npx cypress run --env allure=true --browser chrome
> }
>
> 4. Save the file
> 5. Run : `source .zshrc`
> 6. go to cypress_automation root directory and just run `cyo` for opening cypress with interface or `cyr` to run cypress without interface

## 🏗️ Installation

> * `git clone ssh://git@bitbucket.babel.fr:7999/rfrqa/cypress_automation.git`
> * `cd cypress_automation`
> * `npm install`

## 🌿 Branch naming convention

> * Please prefix your branch name with ont of the following **Bugfix|Hotfix|Feature**.

## ⛩️ Project structure

> * Automated tests FUNCTIONAL DOMAINS :

1. B2C
2. BUY
3. C2C
4. NSE
5. SEARCH
6. SEO
7. TECH
8. VIS

## 🚀 Run test

> * Testing with user interface
 >>
  >> * run command: `npm run cy:open`
>
> * Testing without user interface
>>
  >> *`npm run cy:run`

## 🏅 Code Quality

> * To ensure a high level of code quality in the project and ensure a uniform code formatting rule, the prettier and eslint librairies are used.
> * Please add Prettier extension to your visual code and make sure to add the following configuration to your VS Code configuration :

```json
{
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "editor.formatOnSave": true
}
```

## 📢 Notes

> * In case tests API, The proxy should be set in a terminal before running Cypress:
  >>
  >> * On Linux or macOS: `export HTTP_PROXY=10.110.1.41:8080`
  >> * On Windows: `set HTTP_PROXY=10.110.1.41:8080`
  >>
> * After that, for running e2e testing it's should unset the HTTP_PROXY env variable:
  >>
  >> * On Linux or macOS: `unset HTTP_PROXY`
  >> * On windows: `Remove-Item Env:\HTTP_PROXY`
  >> * Or kill the current terminal and reopen a new terminal

