
npx create-react-app react-ts-demo --template typescript
npm create vite@latest my-react-app --template react-ts

npm i eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin -D


npm i @typescript-eslint/parser @typescript-eslint/eslint-plugin -D

npm i prettier eslint-config-prettier eslint-plugin-prettier -D


安装prettier 
在eslintrc.js中添加
```
"plugin:prettier/recommended"
```


npm i husky -D
npm pkg set scripts.prepare="husky install"
npm run prepare


npx husky add .husky/pre-commit "npm run lint"
npx husky add .husky/pre-commit "npm run format"
npx husky add .husky/pre-commit "git add ."


https://commitlint.js.org/guides/getting-started
commitlint


npx husky add .husky/commit-msg 'npx --no --commitlint --edit ${1}'