title: 用hexo搭建个人博客
date: 2020-09-11 17:50:00
---
 > Windows环境下如何用hexo搭建个人博客？

# 准备环境

 1. 准备好github账号，创建好仓库。
 > https://github.com/demo/demo.github.io.git
 > 注意 demo 的位置，名字必须一样，否则部署不成功
 2. 准备好git环境和node环境，直接官网下载安装即可。

# 安装hexo
> 注：如果是在Windows命令窗口下执行命令需要加 npx，如果是idea下，不需要加。npx 想要解决的主要问题，就是调用项目内部安装的模块
 1. 本地创建一个文件夹，切换目录到新创建的文件夹。以 D:\develop\demo.github.io 为例，要与github仓库名一致
 2. 执行 npm install hexo-cli -g，这一步是安装hexo
 3. 执行命令 hexo init
 > 如果是在Windows命令窗口下执行命令为：npx hexo init，下同
 4. 本地启动：hexo server 或者 hexo s
  > 如果是在Windows命令窗口下执行命令为：npx hexo server
![启动命令](https://img-blog.csdnimg.cn/20200911174042695.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM1OTU2MDQx,size_16,color_FFFFFF,t_70#pic_center)


 5. 本地打开：http://localhost:4000/ 
![启动画面](https://img-blog.csdnimg.cn/20200911174043563.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM1OTU2MDQx,size_16,color_FFFFFF,t_70#pic_center)

# 安装插件
给hexo安装git插件： npm install hexo-deployer-git
>![安装git插件](https://img-blog.csdnimg.cn/20200911174042712.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM1OTU2MDQx,size_16,color_FFFFFF,t_70#pic_center)

安装并配置admin插件：npm install --save hexo-admin
> ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200911174427308.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM1OTU2MDQx,size_16,color_FFFFFF,t_70#pic_center)


下载Next主题：git clone https://github.com/theme-next/hexo-theme-next themes/next
注意有 https://github.com/iissnan/hexo-theme-next 这个地址的主题不再维护，如果使用会有问题，所以避坑。问题如下：
> ![启动错误](https://img-blog.csdnimg.cn/20200911174042708.png#pic_center)
