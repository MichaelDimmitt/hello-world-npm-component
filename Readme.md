## Usage 

Script for the example sourced from: 
https://github.com/MichaelDimmitt/ship-my-component-npm
```bash
## Important for the init command: 
  ## specify the entrypoint: build/index.js  
  ## specify test: webpack 
npm init &&
mkdir build &&
curl -L -o webpack.config.js https://raw.githubusercontent.com/MichaelDimmitt/ship-my-component-npm/master/webpack.config.js &&

npm install react@15.5.4 webpack@2.6.1 && 
npm install -D babel-cli@6.24.1 babel-core@6.24.1 babel-loader@7.0.0 babel-plugin-transform-object-rest-spread@6.23.0 babel-plugin-transform-react-jsx@6.24.1 babel-preset-env@1.5.1 &&
npm test &&
npm publish

## cleanup
rm -rf node_modules package.json package-lock.json webpack.config.js 
```

```javascript
// normal class component implementation is version #7
npm install --save hello-world-npm-component@1.0.7
import HelloWorld from 'hello-world-npm-component';

// functional component implementation is version #6
npm install --save hello-world-npm-component@1.0.6
import { HelloWorld } from 'hello-world-npm-component';
```

## see the code at these two branches:
git checkout react-class-component;
<br/>git checkout react-functional-component;

success reached through the following helpful document:
<br/>https://medium.com/@BrodaNoel/how-to-create-a-react-component-and-publish-it-in-npm-668ad7d363ce
