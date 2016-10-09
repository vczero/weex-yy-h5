
## HOW TO RUN     

```
第一步 安装依赖，建议使用cnpm，没有的话，先安装cnpm
$ cnpm install

第二步 编译.we文件
$ npm run build    

第三步 将所有文件不熟到静态服务器 或者 使用webstorm打开刚项目目录   
使用webstorm预览index.html页面即可

```

## 相对于weex-yy做了哪些修改    
因为weex-yy项目是针对三端环境开发的。有的同学希望不使用源码或者playground就直接看到H5效果，因此，做了如下修改来直接运行H5。      

```
1.增加 package.json、 webpack.config.js 文件     
webpack.config.js 文件的作用主要是将src目录下的所有文件编译成js文件，编译完成的文件放在build目录下。     

2.修改了跳转中的路径，适配到build目录  

3.增加index.html文件，作为H5版本的承载体。Native则是playground

