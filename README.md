# 帕吉网络后台框架
#### 

## 文件目录结构

```
app
├── build // webpack config files 打包配置文件，想修改输出端口，可以更改config.js中的port
├── client - APP 目录结构
│   └── components - 框架组件，包含初始化App组件、顶部导航栏Header组件、侧边栏Sidebar组件、和黑色蒙版Dimmer组件
│   ├── router - 路由配置文件
│   ├── store - Vuex store
│   ├── styles - 全局性的sass配置文件，用于定义全局字体、颜色.此处的sass文件最好不要变更文件位置
│   ├── views - 内部组件，所有的内容组件都放在此文件夹内
│   ├── index.js - 入口文件，里面引入了各项依赖和全局样式文件，请不要更改文件名称
├── dist - build.
├── static - static assets, etc.
├── tests - Your tests
```

## To start:

```bash
 git clone https://github.com/Metnew/vue-element-starter.git vue-project  
 cd vue-project && rm -rf .git
 npm install
 npm run generate_default_styles # run this command to generate default_styles for Element-theme
```


```bash
 npm run generate_theme
```

Now app is ready and you can run it with:

```bash
 npm run dev
```

Make production build:

```bash
 npm run build
```

### Also
PRs, issues, questions, \<something-another> are always welcome.     
Feel free to contact me (or add new issue).

### Author
Vladimir Metnew <vladimirmetnew@gmail.com>

### LICENSE
MIT
