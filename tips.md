> Q: 当我开启 remote js debugging 时一切正常。一旦关闭 debugger 模式后就会报错甚至 crash

##### A: 应考虑 js 兼容性问题。debugger 时 js 运行环境为 chrome，关闭时为 rn 内置环境









> Q: iOS 上的 rn 页面会随着用户手机字体大小变化而变化

##### A: Text 组件提供了禁止缩放方法，具体 props 为 `allowFontScaling: boolean` 如果觉得每次都要设置一次麻烦的话，可以在入口文件处添加如下代码:

```js
Text.defaultProps = Object.assign({}, Text.defaultProps, {allowFontScaling: false});
TextInput.defaultProps = Object.assign({}, TextInput.defaultProps, {allowFontScaling: false});
```





