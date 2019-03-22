# 梧桐车服BSS前端工程

该文件为梧桐BSS端前端项目的基础架构和介绍

## 项目架构版本
| Vue | Element-Ui |
| ------ | ------ |
| v2.5.17 | v3.10 |

| Author | E-mail |
| ------ | ------ |
| 乔宇 | 527324363@qq.com |

## 开发

```bash
# 克隆项目
git clone http://39.105.102.15:8888/firmiana/firmiana_frontend.git

# 安装依赖
npm install

# 建议不要用 cnpm 安装 会有各种诡异的bug 可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# 启动服务
npm run dev

# 打包
npm run dist / yarn run dist
```

## 目录

```bash
├── build                      // 构建相关
├── config                     // 配置相关
├── src                        // 源代码
│   ├── api                    // 所有请求
│   ├── assets                 // 主题 字体等静态资源
│   ├── components             // 全局公用组件
│   ├── directive              // 全局指令
│   ├── filters                // 全局 filter
│   ├── icons                  // 项目所有 svg icons
│   ├── lang                   // 国际化 language
│   ├── mock                   // 项目mock 模拟数据
│   ├── router                 // 路由
│   ├── store                  // 全局 store管理
│   ├── styles                 // 全局样式
│   ├── utils                  // 全局公用方法
│   ├── vendor                 // 公用vendor
│   ├── views                  // views 所有页面
│   ├── App.vue                // 入口页面
│   ├── main.js                // 入口文件 加载组件 初始化等
│   └── permission.js          // 权限管理
├── static                     // 第三方不打包资源
│   └── Tinymce                // 富文本
├── .babelrc                   // babel-loader 配置
├── .eslintrc.js               // eslint 配置项
├── .gitignore                 // git 忽略项
├── .travis.yml                // 自动化CI配置
├── favicon.ico                // favicon图标
├── index.html                 // html模板
└── package.json               // package.json
```

## 其它
  
```bash
# --report to build with bundle size analytics
npm run build:prod

# --generate a bundle size analytics. default: bundle-report.html
npm run build:prod --generate_report

# --preview to start a server in local to preview
npm run build:prod --preview

# lint code
npm run lint

# auto fix
npm run lint -- --fix

#版本号控制
--version change in $store.getters.version from 'src/store/moudules/app.js'
```
  
## D2环境
[D2环境](http://firmiana_frontend.api.d2.yn.cn)

## M1环境
[M1环境](http://firmiana-bss.m1.yunniao.cn)
