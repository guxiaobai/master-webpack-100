# 6-2 如何编写一个 Loader（2）

|本期版本|上期版本
|:---:|:---:
`Thu Sep 15 22:31:24 CST 2022` | -

`webpakc.config.js`

```javascript
resolveLoader: {
  modules: ['node_modules', './loaders']
}
```

### 参考资料

* [resolveLoader](https://webpack.js.org/configuration/resolve/#resolveloader)