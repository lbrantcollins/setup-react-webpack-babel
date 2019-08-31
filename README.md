
# setup-react-webpack-babel

Tyler McGinnis video tutorial:

https://www.youtube.com/watch?v=Zb2mQyQRwqc


`$ npm init -y`
`$ npm install react react-dom`


`$ touch .gitignore`

.gitignore file

`node_modules`.    
`.DS_Store`.    
`dist`


`$ mkdir app`
`$ cd app`
`$ touch index.css index.js`


write the index.js file


install dev (development) dependencies (for building react app)

`$ npm install --save-dev @babel/core @babel/preset-env @babel/preset-react webpack webpack-cli webpack-dev-server babel-loader css-loader style-loader html-webpack-plugin`


webpack: module bundler
 
at the root directory of the project:

`$ touch webpack.config.js`


Add this to package.json

```"babel": {
    "presets": [
      "@babel/preset-env",
      "@babel/preset-react"
    ]
  },
 ```



add a "create" script (used later for production compile)


``` "scripts": {
    "create": "webpack"
  },
```

build to file (index_bundle.js) for production

`$ npm run create`

during development, use webpack-dev-server module    
("open" will open up resulting files in our local server)


``` "scripts": {
    "start": "webpack-dev-server --open"
  },
```
  

build in local cache during development

`$ npm run start`


  

