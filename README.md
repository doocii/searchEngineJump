# searchEngineJump

在线安装 [Greasy Fork](https://greasyfork.org/zh-CN/scripts/27752-searchenginejump)

__说明__
> 5.0.0.0
> 增加设置，可以自行打开关闭搜索列表，两个搜索之间拖动进行排序.
> 拖动排序和有些拖拽手势插件冲突(原因未知), 拖拽手势插件一般按ctrl忽视手势; 排序实质上是交换，两个搜索进行交换。
![例图](http://odp4cbmbx.bkt.clouddn.com/setting20170806230906.png)


已知问题： 与脚本[网页解除限制](https://greasyfork.org/zh-CN/scripts/14146-%E7%BD%91%E9%A1%B5%E9%99%90%E5%88%B6%E8%A7%A3%E9%99%A4)有[冲突](https://greasyfork.org/zh-CN/forum/discussion/21298/x)，开启后，无法进行跳转。可以暂时先用我修改后的[网页解除限制](https://greasyfork.org/zh-CN/scripts/28497-%E7%BD%91%E9%A1%B5%E9%99%90%E5%88%B6%E8%A7%A3%E9%99%A4),大刀阔斧的修改，与原脚本使用上有较大的变化。或者自己修改下原作者的脚本(最简单的修改方式是将unhook_eventNames中的 "mousedown|mouseup" 替换成"click"即可，~~暂时还不知道有什么副作用~~在知乎打开评论列表会跳转到顶部)。


本脚本修改自[searchEngineJump modified version from NLF 4.0.5.3](https://greasyfork.org/zh-CN/scripts/18315-searchenginejump-modified-version-from-nlf)
此类脚本的鼻祖为 NLF 写的 [搜索引擎跳转（searchEngineJump）](http://userscripts.org/scripts/show/84970) , 不过目前该网站已经无法打开， [相关网页快照](http://web.archive.org/web/*/http://userscripts.org/scripts/show/84970)

### 更新历史

> version 5.12.11   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-11-27
- 翻译列表增加海词搜索[感谢建议](https://greasyfork.org/zh-CN/forum/discussion/31670/x)，老用户默认禁用
- 淘宝页面鼠标划过商品后，会遮挡工具栏的问题

> version 5.12.10   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-11-19
- 增加了下载搜索列表, 默认隐藏 [感谢建议](https://greasyfork.org/zh-CN/forum/discussion/31317/x)
- 增加了几个或许将来要用到的设置选项

> version 5.12.9   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-11-04
- 天猫超市导致源网页侧边栏错位的问题 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/30899/)
- 修复上个版本导致知乎固定到顶栏错位的问题

> version 5.12.8   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-10-27
- 淘宝等网站固定到顶栏，会出现错位的问题，依旧有瑕疵。
- 此版本开始火狐用户无法从菜单中直接点击禁用菜单按钮
- 百度页面向上滚动时，隐藏搜索框下面的联想提示

> version 5.12.7   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-10-18
- 修复"固定到顶端"修改后保存，无法及时生效的问题
- 消息提示框位置错误的问题
- 按钮配色，动画微小调整

> version 5.12.6   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-10-10
- 修复图标偏移

> version 5.12.5   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-10-04
- 更改设置后无需重新加载页面
- 设置界面调整： 配色 位置 字体


> version 5.12.4   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-09-23
- 移除 “更多设置-列表排序” 功能，现在可以拖动列表标题排序
- 增加搜索： 购物-闲鱼，mine-GreasyFork 
- 设置界面 图标与名称未对齐的问题

> version 5.12.3   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-09-10
- 设置菜单集成到 Tampermonkey 菜单中
- 点击"设置按钮透明度"后的数字可隐藏设置菜单，重新打开需从Tampermonkey菜单中打开，火狐用户请无视此项更新
- 林花谢了春红，太匆匆 --李煜 相见欢 

> version 5.12.2   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-09-01
- 设置菜单中，被禁用的搜索缺失删除线的问题
- youtube 改版
- 从百度文库跳转时乱码的问题[感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/28783)
- 调整了最低宽度，在一般屏上有更好的表现 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/28783)

> version 5.12.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-27
- 固定搜索栏的情况下，在百度页面二级搜索菜单错位的问题
- 谷歌页面样式微调

> version 5.12.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-21
- 增加post提交方方式 搜索连接后跟‘$post$xx’ 其中的 xx 是指post提交的名称 [相关反馈](https://greasyfork.org/zh-CN/forum/discussion/28440/x)
- 修复“搜索项目”可以与“分类名称”拖拽的问题 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/27907/x)
- 在 searx、搜狗 页面添加样式

> version 5.11.2  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-20
- 设置菜单可视区域过低时，设置按钮 无法自动置底的问题  [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/27907/x)
- 添加雅虎搜索 

> version 5.11.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-19
- 谷歌搜索页面下，“列表排序”间隙过大的问题
- 打磨动画 😂

> version 5.11.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-18
- 增加列表排序的功能：设置-更多设置-列表排序
- ~~修复在 奔跑的奶酪定制版火狐v8 设置菜单错位的问题~~
- 默认隐藏html搜索列表; javlibrary搜索连接修复; 删除百度知道; 增加萌娘百科
- 设置界面样式微调

> version 5.10.3  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-10
- 输入框改为获取焦点后自动选中文本，之前是鼠标点击输入框自动选中文本
- 火狐浏览器设置界面全选的问题
- 必应搜索，“更多设置”菜单错位的问题

> version 5.10.2  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-09
- 设置界面样式调整，增加多个设置按钮。更改设置界面的打开关闭动画

> version 5.10.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-09
- 去除关闭按钮的旋转动画
- 去除莫名多的margin属性

> version 5.10.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-08
- 增加固定到顶端选项,页面向下滚动后工具条能保持在页面顶部。“设置 - 高级 - fixedTop” 改为true, 某些页面兼容的并不是很好 [感谢建议](https://greasyfork.org/zh-CN/forum/discussion/27478/x)

> version 5.9.2  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-07
- 设置菜单可视区域过低时，无法滚动到顶部的问题

> version 5.9.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-06
- 设置菜单可视区域过低时，无滚动条的问题[感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/27907/x)

> version 5.9.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-08-05
- 添加增删搜索列表的功能
- 增加debug 设置-高级-debug (从同类脚本上扒过来的)
- 众多细节调整

> version 5.8.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-07-29
- 依旧无法排除针对某一网站搜索的情况[感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/27527/x)

> version 5.8.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-07-28
- 增加配置文件中rules信息，功能同脚本中的rules一样，但优先级更高,配置文件更新至1.6
- 之前会去掉跳转到当前搜索的搜索，现在会排除搜索引擎针对某一网站搜索的情况 site:xxx.xx [如反馈中的这种情况](https://greasyfork.org/zh-CN/forum/discussion/27527/x)
- 修改本地配置文件后，某些情况下部分信息会被默认配置覆盖的问题


> version 5.7.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-07-26
- 增加修改设置按钮透明度的功能，设置-高级-setBtnOpacity 后面的数字为透明度取值0-1，-1为关闭设置按钮。配置文件更新至1.5
- 删掉配置文件中的details信息，整合到engineDetails中
- 个别网站样式调整

> version 5.6.3  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-07-24
- 修复打开方式无法设置为新标签页打开 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/27413)
- 个别网站样式调整

> version 5.6.2  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-07-23
- 剔除配置文件中无用的信息
- 修复在百度页面打开设置存在的样式问题
- 完善腾讯视频搜索样式

> version 5.6.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-07-20
- 默认添加360搜索,爱奇艺视频及网页顶部搜索栏 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/27278/x)
- 视频分类默认添加腾讯视频搜索，未能实现顶部搜索栏，原因查找中
- 修复网易云音乐跳转默认添加"&type=1" 的问题 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/27196/x)

> version 5.6.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-07-16
- 增加折叠当前搜索分类选项
- 增加配置文件直接修改代码的选项
- 设置界面按钮调整
- 默认隐藏学术搜索列表

> version 5.5.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-06-07
- 添加新的搜索时，图标会优先从google的API获取，网络不通的情况下使用域名加favicon.ico的方式获取 [感谢建议](https://greasyfork.org/zh-CN/forum/discussion/24961/x)
- 细节优化，重置设置时增加询问窗口

> version 5.5.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-06-04
- 增加搜索分类的名称更改的功能
- 设置细节优化

> version 5.4.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-06-01
- 增加对已有搜索列表更改的选项
- 细节优化: 修改设置界面的部分图标和增加部分动画

> version 5.3.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-29
- 增加全局 “新标签页打开” 选项, 配置文件版本改为 1.2

> version 5.2.2  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-28
- 分类中的mine分类(或多个)无法显示的问题

> version 5.2.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-27
- 最多只能添加9个搜索，继续增加无法显示的问题 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/24342/x)
- 更改用户体验：文字不能被选中

> version 5.2.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-20
- 增加添加删除搜索的功能：无容错能力，不会判断你的输入是否正确，搜索连接中的搜索网址需用 %s 替代,添加完后，如需移动，禁用，删除的需要“保存并关闭”然后在设置。

> version 5.1.5  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-14
- 必應錯位 [感謝反饋](https://greasyfork.org/zh-CN/forum/discussion/23528/x)

> version 5.1.4  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-12
- qq音樂網址變更 [感謝反饋](https://greasyfork.org/zh-CN/forum/discussion/23366/x)

> version 5.1.3  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-11 
- 上一个版本忘改版本号就发布出去(改版本後，greasyfork無視僅有版本號的更新)
- 翻譯(百度，谷歌，必應，有道都有所調整)小調樣式 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/23297/x)

> version 5.1.2  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-11 
- 由于上个版本的修改导致，从百度主页搜索无跳转栏的问题

> version 5.1.2  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-11 
- 从谷歌主页搜索后刷新页面，跳转栏丢失的问题 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/23230/x)
- 网速不好的情况下，从谷歌主页搜索无样式的问题

> version 5.1.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-10 
- 添加动画效果
- 将设置改为弹性布局(测试)

> version 5.1.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-10 
- 增加修改源网页的能力，用以兼容脚本
- 与Google Variety样式不兼容的问题
- google搜索页面中样式微调
- 配置文件的版本无法自动更新问题

> version 5.0.5  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-10 
- 添加搜狗知乎搜索 [感谢建议](https://greasyfork.org/zh-CN/forum/discussion/23140/x)
- 添加搜狗微信搜索 (在分类 mine 中)
- 本地数据存储版本升级为 1.1

> version 5.0.4  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-9 
- 5.0.0.2中与样式“Google Variety”不兼容问题修改后弊大于利，暂时改回去

> version 5.0.3  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-09 
- 设置中无法保存新标签页打开的问题
- 修复因为5.0.0版本导致谷歌、百度从主页搜索无法显示跳转栏的问题
- 添加名为“rwl-exempt”的class，为解决与脚本【网页解除限制】做准备
- 版本由 5.x.x.x 改为 5.x.x

> version 5.0.0.2  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-09 
- 更改字体设置后会造成错位 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/23109/x)
- 与Google Variety样式不兼容 

> version 5.0.0.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-08 
- 注释掉 console.log

> version 5.0.0.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-08 
- __添加设置菜单(测试)__ 自定义开关搜索列表，排序，无法自己添加。测试版本
- 添加果壳搜索
- 修复 duckduckgo 样式


> version 4.1.1.17  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-05-1 
- 添加脚本图标
- 百度音乐样式不居中 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/22341/x)
- 名称从 “searchEngineJump” 改为 “searchEngineJump 搜索引擎快捷跳转”

> version 4.1.1.16  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-04-23 
- 修复从百度，谷歌主页搜索时没样式的问题

> version 4.1.1.15  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-04-23 
- acfun 样式不居中 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/22066/x)

> version 4.1.1.14  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-04-21 
- 修复上个版本导致的搜索栏遮挡联想词的问题

> version 4.1.1.13  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-04-20 
- 谷歌搜索工具被遮挡的问题 [感谢反馈](https://greasyfork.org/zh-CN/forum/discussion/22006/x?locale=zh-CN)

> version 4.1.1.12  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-04-09 
- 修复上一个版本更改动画造成列表偏移的问题

> version 4.1.1.11  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-04-07 
- 更改退出动画，使看上去更流畅

> version：4.1.1.10  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-04-05 
- 谷歌翻译改hk为com
- 百度搜索改为他们自己ajax请求，不再强制刷新网页

> version：4.1.1.9  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-04-03 
- 修复b站样式，调整搜索连接
- 样式小调

> version：4.1.1.8  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-03-31 
- 修复flickr样式
- 修复维基百科无法获取搜索词的问题
- 百度联想搜索后样式丢失的问题，虽然样式不再丢失，但是鼠标划过后详细搜索列表依旧没有，可以修复，但是扯得地方太多，以后版本搞，此版本上的修复更大意义上是面子工程。
- 图标微调：youtube 网易云音乐 维基百科

> version:4.1.1.7  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-03-31 
- 可以在部分开启 Content Security Policy (CSP) 安全策略的网站上使用，知乎可以，github依旧不行
![知乎开启成功](http://odp4cbmbx.bkt.clouddn.com/%E7%9F%A5%E4%B9%8E20170331174102.png)

> version:4.1.1.6  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-03-29 
- 添加 Pinterest, MDN 搜索
- 部分图标改为 32x32 ，16X16锯齿太明显,图标微调：百度

> version:4.1.1.5  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-03-21 
- 统一图标 16x16 base64编码,为此专门写个工具 [img2base64](http://iqingxin.cn/tool/)

> version:4.1.1.4  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-03-20 
- 修复个别网页搜索关键字编码问题
- 修复样式盖过百度搜索框的问题
- 字体颜色改为 #333

> version:4.1.1.3  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-03-20 
- 修复音悦tai搜索连接

> version:4.1.1.2  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-03-10 
- 修复百度 "相关搜索" 样式丢失的问题
- 添加 GitHub 搜索

> version:4.1.1.1  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-03-06 

- 修复百度搜索页面,翻页后样式丢失的问题
- 修复 youtube 页面,左侧遮挡的问题
- 修复 acfun 样式丢失的问题
- 还有好多问题, 慢慢来
![youtube遮挡](http://odp4cbmbx.bkt.clouddn.com/youtube3-6.png)


> version:4.1.1.0  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2017-03-05: 
- 修复使用百度搜索后,页面丢失样式的问题,方法较粗暴
![问题图片](http://odp4cbmbx.bkt.clouddn.com/%E9%97%AE%E9%A2%98.png)


> 2017-2-28:upload version:4.1.0.0

![例图](http://odp4cbmbx.bkt.clouddn.com/searchEngineJump.png)
