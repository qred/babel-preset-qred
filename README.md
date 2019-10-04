# babel-preset-qred

## Usage

### 1. Install babel

Run:
```bash
yarn -D babel-loader @babel/core
```

### 2.  Configure babel

Create a file named `.babelrc` with the following contents in the root folder of your project:

```js
{
  "presets": ["qred"]
}
```

### 3. Configure webpack

In your `webpack.config.js` add the following section:

```js
module: {
  rules: [
    {
      test: /\.jsx?$/,
      exclude: /node_modules/,
      loader: "babel-loader"
    }
  ]
}
```
