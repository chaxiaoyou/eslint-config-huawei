# eslint-config-huawei
[![npm](https://img.shields.io/npm/v/eslint-config-huawei.svg)](https://www.npmjs.com/package/eslint-config-huawei)
[![npm](https://img.shields.io/npm/dt/eslint-config-huawei.svg)](https://www.npmjs.com/package/eslint-config-huawei)
[![Build Status](https://travis-ci.org/sept08/eslint-config-huawei.svg?branch=master)](https://travis-ci.org/sept08/eslint-config-huawei)
[![codebeat badge](https://codebeat.co/badges/eb2806d1-5060-418a-b532-12f4a029646f)](https://codebeat.co/projects/github-com-sept08-eslint-config-huawei-master)

> Huawei Eslint rules

# 规则列表
*   基本规则：  "eslint-config-huawei"
*   vue规则：   "eslint-config-huawei/vue"

# 规则说明
规则设置文档可参阅(待完善)[wiki](https://github.com/sept08/eslint-config-huawei/wiki)
暂时可参阅配置文件：
*  [基本配置](https://github.com/sept08/eslint-config-huawei/blob/master/index.js)
*  [Vue配置](https://github.com/sept08/eslint-config-huawei/blob/master/vue.js)

# 使用说明
## 基本规则
### 安装
``` shell
npm install --save-dev eslint eslint-config-huawei babel-eslint
```
### 配置方法
在项目根目录下创建`.eslintrc.js`，并复制以下内容：
``` javascript
module.exports = {
  extends: [
    'eslint-config-huawei',
  ],
  globals: {
    // 项目需要的全局变量，false指定变量为只读：
    //
    // _: false,
    // $: false
  },
  rules: {
    // 项目自定义规则配置
  }
};
```


## Vue规则
### 安装
``` shell
npm install --save-dev eslint eslint-config-huawei babel-eslint eslint-plugin-vue@next vue-eslint-parser@2.0.1-beta.2
```
### 配置方法
``` javascript
module.exports = {
  extends: [
    'eslint-config-huawei/vue',
  ],
  globals: {
    // 项目需要的全局变量，false指定变量为只读：
    //
    // _: false,
    // $: false
  },
  rules: {
    // 项目自定义规则配置
  }
};
```

## VSCode配置
### 安装eslint插件
`Ctr+Shift+X`打开Extensions，搜索ESlint并安装，重启VSCode
### 配置
`File-->Preferences-->Settings`或`Ctrl + Comma`打开设置文件`settings.json`，添加如下配置
``` javascript
// 检查文件类型
"eslint.validate": {
  "javascript",
  "vue"
}
```
