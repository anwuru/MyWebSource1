---
title: git与Hexo使用中的常见问题
date: 2023-04-29 21:13:19
tags: 
- 学习笔记
- 博客搭建
- 命令行
---

#### hexo d上传失败 改用hexo d -g解决

-g是全局的意思？

参见：[hexo d 报错 hexo 安装搜索功能 hexo 报错没有git_hexo安装4058问题_0x8g1T9E的博客-CSDN博客](https://blog.csdn.net/sirobot/article/details/110630662)

其他：

[(7条消息) git:上传代码时，出现fatal: unable to access ‘XXX‘: Recv failure: Connection was reset 错误解决方法（保姆级教学）_王王小小酥o的博客-CSDN博客](https://blog.csdn.net/m0_69087087/article/details/128838186)



[Hexo部署出现错误 Error: Spawn failed 解决方式 | 毋忘草的小岛 (myosotis.xin)](https://www.myosotis.xin/2021/08/25/hexo-8/)

```bash
##进入站点根目录

##删除git提交内容文件夹
rm -rf .deploy_git/

##执行
git config --global core.autocrlf false

##最后
hexo clean && hexo g && hexo d
```



猜测大概率是网络问题，不做更改重试多次也能成功

好像不开clash代理才能推送？



#### 使用Yilia主题，本地可显示，但推送后头像不能显示

![image-20230429235013282](https://s2.loli.net/2023/04/29/ADvYfWT4Zh9SyUV.png)

怀疑是没有权限访问更深层的目录？

将/assets/blogImg/touxiang.png改为了/touxiang.png后解决

参见主题作者在项目回答中给出的回复



#### 书写代码时不能忘记代码冒号后面的空格



#### git命令行使用时如何[use arrow keys](https://www.cnblogs.com/crazycode2/p/10125901.html)使用不了方向键选择

在使用主题时遇到

举例三行三个选项

```
> A
  B
  C
```

回车时光标在哪一行上面，选中哪一行

在A行回车选择B

网上有说手动输入>，没有成功。

用win自带的命令行貌似可以，未尝试。



#### 命令行书写TIPS

上下是历史记录



