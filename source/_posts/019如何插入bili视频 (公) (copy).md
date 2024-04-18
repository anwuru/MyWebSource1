---
title: 如何插入bili视频
date: 2023-4-29 21:41:05
tags: 
- 博客搭建
- 待办
---

[标签插件（Tag Plugins） | Hexo](https://hexo.io/zh-cn/docs/tag-plugins)



[Hexo博客中加入Bili标签插件添加视频 (baidu.com)](https://baijiahao.baidu.com/s?id=1624368667577594763&wfr=spider&for=pc)

[hexo博客添加bilibili外链视频 | 烟雨陌上云霄 (yymsyx.com)](https://yymsyx.com/Ming/b183ff03/)

[hexo博客插入B站视频外链（标签插件实现）_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1Cb411677C?p=2&vd_source=f141f5927a7a467023f63b2fbdf6420c)

[hexo博客插入B站视频外链（raw实现）&（标签插件实现）_哔哩哔哩_bilibili](https://www.bilibili.com/video/av42467871/?vd_source=f141f5927a7a467023f63b2fbdf6420c)

[11.外挂标签的添加_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1pt4y1n7kX/?from=search&seid=7707160123730220135&spm_id_from=333.337.0.0&vd_source=f141f5927a7a467023f63b2fbdf6420c)

代码块示例：

```
{% raw %}

<div style="position: relative; width: 100%; height: 0; padding-bottom: 75%;">
<iframe src="//player.bilibili.com/player.html?aid=42467871&bvid=BV1Cb411677C&cid=74518845&page=2" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" style="position: absolute; width: 100%; height: 100%; Left: 0; top: 0;" ></iframe></div>

{% endraw %}
```

```
 {% raw %}
<div style="position: relative; width: 100%; height: 0; padding-bottom: 75%;">
    <iframe src="//player.bilibili.com/player.html?aid=206890880&bvid=BV1Ah411z7Po&cid=378344365&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" style="position:absolute; height: 100%; width: 100%;"> </iframe>
</div>
{% endraw %}
```

{% raw %}{% endraw %}貌似是防止转换中受影响的？

html可以直接在md里放出来，不要用代码块包裹，这里只是示例所以用了代码块

{% raw %}

<div style="position: relative; width: 100%; height: 0; padding-bottom: 75%;">
<iframe src="//player.bilibili.com/player.html?aid=42467871&bvid=BV1Cb411677C&cid=74518845&page=2" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" style="position: absolute; width: 100%; height: 100%; Left: 0; top: 0;" ></iframe></div>

{% endraw %}

 {% raw %}
<div style="position: relative; width: 100%; height: 0; padding-bottom: 75%;">
    <iframe src="//player.bilibili.com/player.html?aid=206890880&bvid=BV1Ah411z7Po&cid=378344365&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" style="position:absolute; height: 100%; width: 100%;"> </iframe>
</div>
{% endraw %}
