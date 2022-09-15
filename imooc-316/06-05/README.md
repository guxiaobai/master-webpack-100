# 6-5 Bundler 源码编写（模块分析 2）

|本期版本|上期版本
|:---:|:---:
`Fri Sep 16 00:06:14 CST 2022` | -


```js
const dependencies = {};
traverse(ast, {
  ImportDeclaration({node}){
  	const dirname = path.dirname(filename)
  	const newFile = './' + path.join(dirname, node.source.value)
  	dependencies[node.source.value] = newFile;
  }
})
```

```js
{
	'./message.js': './src/message.js'
}
```