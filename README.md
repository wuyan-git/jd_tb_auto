# 618||双十一||淘宝||京东||赚喵币||赚金币任务自动完成脚本
基于AutoJs编写的618||双十一||淘宝||京东||赚喵币||赚金币任务自动完成脚本

# 重要说明

- TB的有代码，但是因为检测无障碍的原因导致做完任务获得的金币数量100-200，找不到解决方法
- JD正常使用

# 更新

2021-06-08

1.【TB618】上传TB自动化代码 注：使用该脚本极大概率获得金币为100（反正我是的，我这里提供脚本，如果解决TB检测无障碍的问题交给你们了）

2.【JD618】更改少量不合理注释

2021-06-07

1.【JD618】添加日志打印窗口

2.【JD618】添加自动判断程序是否卡在某个界面

注：JD需要手动进入到活动界面

2021-06-06

1.【JD618】上传JD自动化代码，比较简单，不提供打包apk

# 另外

可能每天会有不同的活动，我这里做了一个需要做的活动和不需要做的活动列表，如果自己发现程序没更新，可以自己在代码里面添加

```js
// 需要忽略的任务中包含的关键字
const IGNORE_LIST = ['好友','成功入会','加入战队','参与可得2000金币'];
// 点击之后返回的任务
const BACK_LIST = ['浏览并关注','逛店可得','成功浏览可得1000金币'];
// 去完成按钮
const GO_FINISH = '去完成';
// 需要做的任务
const FINISHED_TASK = ['您所访问的页面不存在','全部完成啦',/获得\w+金币/,'已浏览'];
```

比如我这里忽略了入会的那个活动，就把那个任务的关键字“成功入会”放在了IGNORE_LIST的变量里面，又比如有的活动是点进去直接返回就行，这里也有进行判断的列表-BACK_LIST，只需要把任务的关键字加入即可。



~~高版本淘宝有制裁规则，会监控auto.js等脚本app进程，奖励会变得特别低<br>~~
~~亲测淘宝V9.5.7版不会监控进程，可以获得全额奖励，推荐使用此版本<br>~~
~~<a href="https://www.wandoujia.com/apps/32267/history_v278"><span>淘宝9.5.7下载</span></a><br>~~
~~感谢@hyue418~~
~~项目地址：https://github.com/hyue418/taobao-11-11~~
~~<br>~~
~~使用方法：<br>~~
~~1、https://zhuanlan.zhihu.com/p/90065914 根据这个文章安装好AutoJs，将代码导进去，然后设置无障碍服务运行即可。<br>~~
~~2、直接安装打包好的apk，安装完毕设置好无障碍服务运行即可。<br>~~

# ~~如何关闭<br>~~
~~直接cut掉后台进程即可。~~
~~<br>~~
~~<br>~~
# ~~更新日志~~
~~2020年11月4日：更新TB。~~
~~2020年11月2日：很久没更新了。。这几天没什么时间，就没搞了，然后JD版本的搞不好，去找其他大佬吧。。<br>~~
~~2020年10月26日：新增JD全民营业；优化部分代码。（PS：昨天看比赛去了，没看到有JD这个活动，今天下班然后补充了第一个版本。<br>~~
~~2020年10月25日：修改bug。（看比赛看比赛）<br>~~
~~2020年10月24日：优化部分代码,然后发现了TB有对auto.js进行制裁的问题，在网络上找到个版本防制裁。<br>~~
~~2020年10月23日：修复进入淘宝特价界面的时候无法继续运行。（PS:我自己本机是没问题的，如果有问题明天再修复，噢对了是今天。。不小心过了一天了）<br>~~
~~2020年10月21日：双十一活动开始了，我又来了，（其实是提醒我才知道的hhhh）。<br>~~
~~<br>~~
~~<br>~~
~~2020年5月24日：这是一个初步测试的Demo，目前存在的问题是，有些任务需要人工点击，因为只有一个帐号无法顾及全部可能性，后续会不断更新。<br>~~
~~2020年5月25日：十点下班回来弄了下，早上发给朋友测试发现报错了，原来出了个逻辑问题，加个continue就能解决。然后自己又跑了遍，添加了一些活动操作，明天继续。<br>~~
~~2020年5月26日：再次跑完一遍活动并且解决了部分问题和加入了我目前遇到的活动页面操作，因为每天只能测一个号，改完之后也没进行第二次测试。这次加了写日志代码方便调试，有兴趣的朋友可以去调试下。<br>~~
~~2020年5月27日：修复小bug，基本能跑完全程，可能有些活动界面没覆盖到所以手动点一下也可。还有就是昨天打包的那个apk打包错了导致用不了，早上才发现。<br>~~
~~2020年5月28日：修复购物车bug，新加两个活动页面操作。（感谢网友使用并且issue~^^）<br>~~
~~2020年5月30日：JD的基本没啥问题了吧？有问题我会及时修改。然后我发现TB也开始了。。。于是我顺便把TB的也写进来，至于标题我就不改了，用文件夹分开。还没完成，因为写着写着TB那个页面出现了BUG，没办法继续写。<br>~~
~~2020年5月30日：根据网友提议改了点代码，tb的也做了第一个版本，但不是很稳定（我自己试了一个号而已）？还有JD那个金币小人也弄了个版本，没做到一起，有能力的朋友可以整到一起。<br>~~
~~2020年5月31日：可能由于手机和app版本问题，出现了不能适配的情况，如果脚本不能自己进入叠蛋糕界面的话可以先自己打开app进入到活动界面。<br>~~
~~2020年6月3日：这两天有点忙就没怎么改，今天哦不，昨天早下班就改了下，然后添加了一个界面，但是打包之后运行不了，我先把代码提交吧，安装包的问题再看，可以用AutoJS运行代码。<br>~~
~~2020年6月6日：周末维护更新<br>~~
~~2020年6月10日：更新了JD的，最近使用比较不稳定，而且多了个开会员的活动，我没有将那个活动写进去，因为感觉直接开卡比较不好，如果有需要的话我再做另一版有开会员活动的。<br>~~
~~2020年6月16日：更新了JD和优化了TB，有个兄弟说JD没办法自动进入到活动界面，可以在首页进入，但是首页那个我写了之后，代码是有反映但是就是没办法进去，所以我就不解决了，只能自己手动进入到活动界面了。<br>~~
~~2020年6月19日：活动结束~感谢朋友们的40个start，以后有类似的活动会继续更新 bye<br>~~