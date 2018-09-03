# vue-cli 生成的项目配置 px2rem

## 动态计算html的fontsize
```
html {
  font-size: calc(100vw / 3.75);
}
```

## `.postcssrc.js`添加`postcss-pxtorem`配置

### 安装
```
npm i postcss-pxtorem -D
```
### 配置
```
module.exports = {
  "plugins": {
    "postcss-import": {},
    "postcss-url": {},
    // to edit target browsers: use "browserslist" field in package.json
    "autoprefixer": {},
    "postcss-pxtorem": {
      rootValue: 100, //默认根目录字体大小(px)
      unitPrecision: 5, //保留小数位
      propList: ['*'],
      // selectorBlackList: [''], //过滤的类名
      replace: true, //默认直接替换属性
      mediaQuery: false,
      minPixelValue: 6, //所有小于设置的样式都不被转换
    }
  }
}
```
