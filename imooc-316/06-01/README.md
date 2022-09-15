# 6-1 如何编写一个 Loader（1）

|本期版本|上期版本
|:---:|:---:
`Thu Sep 15 22:18:51 CST 2022` | -


1 - `loaders/replaceLoader.js`

```javascript
module.exports = function(source){
  return source.replace('gu', 'guxiaobai')
}
```

2 - `webpakc.config.js`

```javascript
use: [path.resolve(__dirname, './loaders/replaceLoader.js')]
```


### 参考资料

* [Loader Interface](https://webpack.js.org/api/loaders/)
* [loader-utils](https://github.com/webpack/loader-utils)
