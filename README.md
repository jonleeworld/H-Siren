### 主题前言

用 WordPress 来做博客程序完全是因为一款主题呢！  
嗯，就是博主现在用的，由 [蜜汁路易](https://www.cssplus.org/ "蜜汁路易") 二次修改发布的 Siren 主题！
它的前身就是由 [Fuzzz](http://fui.im/ "Fuzzz") 制作的 Akina 主题。

首先感谢他们的作品呢……

因为博主超喜欢单栏主题的设计，还有 PJAX 加载，所以博主一直就在打磨这款主题中……  
（当然是根据自己喜欢的口味来更改滴啦）  
学长是个细节控，代码洁癖，某些强迫症集一身的人啦……  
（才不是处女座呢，学长是风象天秤座的）  
所以在打磨这款主题在细节处纠结了 N 多遍后才能有决定的说……  

嗯，好作品感觉就是要分享出去才行呢……  
~~（自己封的好作品称号，2333）~~  
对比 Siren 最后更新版本的修改，就摘几条重要的地方来说下吧……  

### 主题修改

- 任何页面背景头图可以选择使用随机图片API显示，比如 [漫月API](https://random.ikmoe.com/ "漫月API")
- PC 端首页的博主描述，可以选择使用“一言”代替，由 [Hitokoto - 一言](http://hitokoto.cn/ "Hitokoto - 一言") 支持
- 修正菜单栏显示效果：PC 端清晰可见了，移动端文字加大和居中显示
- 主页文章列表修改图文风格为卡片式风格，新视觉！
- 集成 Live2D 看板娘，支持刷新换装
- 加深文章内容文字颜色和增大字体，阅读不费眼了
- 收窄 PC 端正文显示区域的最大宽度和评论列表的最大宽度
- 简化评论 UA 信息，显示效果修改为划过评论才显示
- 评论者的连接添加了页面跳转，不会在当前窗口加载了
- 评论框添加了表情，并支持实时预览；由 [小さな手は](http://www.littlehands.site/ "小さな手は") 实现，效果很好，谢谢他
- 重写友链页面，样式与代码提取自 [DIYGod](https://diygod.me/ "DIYGod") 的 [Amativeness](https://github.com/DIYgod/Amativeness "Amativeness") 主题
- 原生编辑器添加载入主题样式，后台写文章可视化与前台显示效果一致
- 后台屏蔽 WordPress 更新与编辑器自动保存等……
- 添加鼠标点击特效
- 添加网页运行天数
- 添加 ICP 备案号选项
- 添加谷歌分析代码输入框
- 添加屏蔽鼠标右键
- 添加浏览器标签焦点判断
- 添加复制友情提示

**多数添加的功能均有开关可以自行选择是否启用！**

### 功能介绍

#### 卡片式风格

主页文章列表的装饰图支持随机图片API，并使用 MD5 24位随机数载入，大几率减少重复图片的现象；  
显示条件判断如下：  
1. 文章设置有特色图，则显示该特色图；
2. 如果第一条不成立，则随机显示主题默认的十张图；（重复显示的几率较高）
3. 如果第一条不成立，如果开启了 **随机装饰图** 选项，并且添加了 **背景图API** 的连接，则会覆盖第二条；

#### 随机装饰图

文章页与页面的头部装饰图，也支持调用随机图片API，写文章和发页面可以不用专门挑选与添加特色图了，  
也不用看到没有特色图的文章页和页面光光秃秃的样子了……  
显示条件判断如下：  
1. 文章设置有特色图，则显示该特色图；
2. 如果第一条不成立，则不显示特色图！（与上面不一样的地方）
3. 如果第一条不成立，如果开启了 **随机装饰图** 选项，并且添加了 **背景图API** 的连接，则会覆盖第二条；

### 现有问题
> 某些屏蔽邮件发送的主机可能会导致评论后 AJAX 刷新严重超时的问题。  
某些主机上使用主题会导致个别界面错位。

### 获得主题
前往我的 [Github](https://github.com/galnetwen/H-Siren "Github") 去狠狠地 Star 吧！![](https://haremu.com/wp-content/themes/Siren/OwO/images/emoticon_002.png)  
为了名称美观，下载 zip 压缩包的朋友请把解压出来的文件夹改下名字，改为 **H-Siren** ！

### 注意事项

使用友链页面需要新建 LINK 和 BANS 两个分类，其中 BANS 分类用于显示崩坏掉的却暂时不撤销的友链。  
新添加的友链要放进这两个分类里面，友链才可以看见噢 ~

### 更新日志
**2018.01.08**
- 修复某些浏览器点击回复别人的评论时，页面滑动错误；点击回复不再需要下拉页面找输入框了
- 修复发布版本 Live2D 无法启动的问题

**2018.01.09**
- 修正友链模板中默认头像的图片路径
- 友链分类添加判断，没有友链时不显示友链分类元素

**2018.01.10**
- 添加管理员前台 AJAX 删除评论的功能
- 修改移动端评论列表评论时间的显示效果

**2018.01.14**
- 移除难看烦人的 ServerChan 微信推送
- 添加图片放大功能，在文章页设置中开启
- 修正 卡片式风格 在没有正文内容时的显示效果

**2018.03.21**
- 尝试修复评论表情框在某些主机无法加载的问题

**2018.04.07**
- 新增一个 “高斯模糊” 网页背景风格 样式，在基本设置中选择，效果仅限于 PC 端
- 修正主题样式部分小细节的参数，强迫症 OJ8K

**2018.04.10**
- 修复网页运行天数的 BUG ，需要在后台重新填写建站日期格式  

### 主题欣赏

**白色简约**

![](https://haremu.com/wp-content/uploads/2018/01/20180110051930.jpg)
![](https://haremu.com/wp-content/uploads/2018/01/20180110052048.jpg)
![](https://haremu.com/wp-content/uploads/2018/01/20180110052201.jpg)
![](https://haremu.com/wp-content/uploads/2018/01/20180110052250.jpg)
![](https://haremu.com/wp-content/uploads/2018/01/20180110052347.jpg)
![](https://haremu.com/wp-content/uploads/2018/01/20180110052418.jpg)
![](https://haremu.com/wp-content/uploads/2018/01/20180110052542.jpg)

**高斯模糊**

![](https://haremu.com/wp-content/uploads/2018/01/20180407133429.png)
![](https://haremu.com/wp-content/uploads/2018/01/20180407133535.png)
![](https://haremu.com/wp-content/uploads/2018/01/20180407133728.png)
![](https://haremu.com/wp-content/uploads/2018/01/20180407142300.png)
