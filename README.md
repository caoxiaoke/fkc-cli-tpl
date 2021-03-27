# fkc-cli-tpl

一个脚手架，通过交互式命令从Gitlab、 Github中下载模版代码生成新项目，不需要每次都配置项目脚手架，也不需要每次都copy 原来项目文件，删删减减。

**安装**

```javascript
npm i fkc-cli -g
```

<br/>

输入「fkc」了解脚手架

```javascript
fkc
```
[![fkc-cli](https://user-images.githubusercontent.com/12712339/112712511-12567400-8f0b-11eb-9ef5-1a9a4427b2a4.png "fkc-cli")](https://user-images.githubusercontent.com/12712339/112712511-12567400-8f0b-11eb-9ef5-1a9a4427b2a4.png "fkc-cli")

<br/>

**查看所有模版**

```javascript
fkc-cli
```
[![fkc](https://user-images.githubusercontent.com/12712339/112713035-e4266380-8f0d-11eb-9b18-3b764662831e.png "fkc")](https://user-images.githubusercontent.com/12712339/112713035-e4266380-8f0d-11eb-9b18-3b764662831e.png "fkc")
<br/>

**创建项目**

```javascript
fkc init react-vw-layout demo-project
```

[![fkc](https://user-images.githubusercontent.com/12712339/112713310-7da24500-8f0f-11eb-8b0d-7c64590157d5.png "fkc")](https://user-images.githubusercontent.com/12712339/112713310-7da24500-8f0f-11eb-8b0d-7c64590157d5.png "fkc")
<br/>

**项目创建完毕**

[![fkc](https://user-images.githubusercontent.com/12712339/112713407-c35f0d80-8f0f-11eb-8c09-a897e8692291.png "fkc")](https://user-images.githubusercontent.com/12712339/112713407-c35f0d80-8f0f-11eb-8c09-a897e8692291.png "fkc")


<br/>

**fkc-cli 脚手架参考**

**脚手架的作用**

1. 减少重复性的工作，不需要复制其他项目再删除无关代码，或者从零创建一个项目和文件。 
2. 可以根据交互动态生成项目结构和配置文件。 
3. 多人协作更为方便，不需要把文件传来传去。 


**参考思路**

1. 项目模板放在Gitlab、 Github上 。
2. 用户通过命令交互的方式下载不同的模版 。
3. 经过模版引擎渲染定制项目模版 。
4. 模版变动，只需更新模版即可，不需要用户更新脚手架 。

**设计模块知识点**

1. commander.js命令行工具 。
2. download-git-repo: 用来下载远程模板 。
3. inquirer: 交互式命令行工具 。
4. ora: 显示loading动画 。
5. chalk: 修改控制台输出内容样式 。
6. log-symbols: 显示出 √ 或 × 等的图标 。

<br/>
来源：https://blog.csdn.net/sinat_17775997/article/details/106679808
