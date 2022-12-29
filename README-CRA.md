https://brygrill.medium.com/create-react-app-with-typescript-eslint-prettier-and-github-actions-f3ce6a571c97


npx create-react-app modal-animations-it-sinyak2 --template typescript

ESLint
Install the ESLint packages for TypeScript and Jest support.
Note, ESLint is installed with create-react-app, so you don’t need to explicitly install it.

npm i -D @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-config-airbnb-typescript eslint-plugin-jest

npx install-peerdeps --dev eslint-config-airbnb

Prettier
Next, add the packages to integrate ESLint with Prettier rules.

npm i -D prettier eslint-config-prettier eslint-plugin-prettier

"scripts": {
"format": "prettier --write src/**/*.ts{,x}",
"lint": "tsc --noEmit && eslint src/**/*.ts{,x}"
}

