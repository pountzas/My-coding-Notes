# Insallation
## Es Lint
### JS
```
npm install --save-dev eslint@7.x eslint-config-airbnb-base@14.x eslint-plugin-import@2.x babel-eslint@10.x
```

### React
```
npm install --save-dev eslint@7.x eslint-config-airbnb@18.x eslint-plugin-import@2.x eslint-plugin-jsx-a11y@6.x eslint-plugin-react@7.x eslint-plugin-react-hooks@4.x @babel/eslint-parser@7.x @babel/core@7.x  @babel/plugin-syntax-jsx@7.x  @babel/preset-react@7.x @babel/preset-react@7.x
```

## Style Lint
#### JS, React
```
npm install --save-dev stylelint@13.x stylelint-scss@3.x stylelint-config-standard@21.x stylelint-csstree-validator@1.x
```
#### check for errors<br>
```
npx eslint .
```
```
npx eslint . --fix
```
```
npx stylelint "**/*.{css,scss}"
```
```
npx stylelint "**/*.{css,scss}" --fix
```

### Errors on heroku

#### Failed to load config "airbnb" to extend from. Referenced from:

```
rm -rf node_modules
npm install eslint --save
npm install eslint-config-airbnb-base --save
npm install eslint-plugin-markdown --save
npm install eslint-plugin-import --save
npm i
npx eslint --version
```
