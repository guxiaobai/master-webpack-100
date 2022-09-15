# 6-3 如何编写一个 Plugin

|本期版本|上期版本
|:---:|:---:
`Thu Sep 15 23:21:50 CST 2022` | -


1 - `plugins/copyright-webpack-plugin.js`

```js
class CopyrightWebpackPlugin{
	constructor(options){}
	
	apply(compiler){
	}
}
module.exports = CopyrightWebpakcPlugin;
```

2 - `webpack.config.js`


```js
CopyrightWebpackPlugin = require('./plugins/copyright-webpack-plugin.js')

plugins: [
	new CopyrightWebpackPlugin()
]
```

```bash
debug: 'node --inspect-brk ./node_modules/webpack/bin/webpack.js'
```

## Ref

* [https://webpack.js.org/api/compiler-hooks/](https://webpack.js.org/api/compiler-hooks/)