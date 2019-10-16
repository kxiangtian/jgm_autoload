# jgm_autoload

3.6 修复了政策中心升错政策的bug,感谢NGA水友 tannium 。
紧急修复了换装3.5中第一行少一个'的错误。

大家期待的界面已经有了，不过我没找到怎么发布界面的方法，只能自己用。
由于界面的便捷性，以后两个系列将合并为一个版本。

4.0

增加了设置界面

1.自动收钱

工业、商业、住宅三行可以分别设定

2.自动升级

现在可以同时升级2个建筑，建筑的标记为
第一行：工业7，8，9
第二行：商业4，5，6
第三行：住宅1，2，3

3.政策升级

可以自动找到你现在的阶段。
你可以指定这一阶段的5个或者4个选项的优先升级顺序
任意阶段政策的标记顺序为：
1 2
3 4
5
优先逻辑为：按选择的优先顺序依次升满，如果到所填的优先级都不能升，则自动寻找可升级的第一个选项。

4.货物成色选择

可选：只收橙、收橙紫、全收；
选择逻辑为：
只要选中“全收”，则全收，其他选项选中也无效；
只要选中“收橙紫”，则“只收橙”选中无效

5.一键换装

自动在收货前切换至收货配置，收完货切回收钱配置。
换装逻辑为：先检查某个位置的两种配置是否一致，如果不一致再更换。然后检查目标建筑是否已在位置不需要更换。最后，如果找不到更换目标，跳过进行下一个

*********************************************************

一共三个系列:一件换装版本，不换装只收火车版本，开红包。
由于历史遗留问题，名称比较混乱。请大家使用最新版。
前两个系列同步更新，最新版3.5。
开红包最新版2.1，应该不需要再更新了。

一. 家国梦云手机版一件换装版3.6
3.6 修复了政策中心升错政策的bug,感谢NGA水友 tannium 。

3.5

修复了字库中的错误，现在机械企鹅和媒体之声可以正确识别了
修复了政策中心和更换建筑时翻页的死循环
修复了政策中心的一处坐标错误

3.4

怎么说呢，又一次修复了进入政策中心卡死的BUG

3.3 

1. 初步优化了一键换装的逻辑，现在可以自动识别该位置是否需要换建筑了。
2. 进一步延长了重启游戏的延时到15秒，以避免意外的卡顿造成在登陆页面点击的众多BUG，未来将进一步优化防卡顿逻辑。


3.2 

新增指定政策优先升级，修复了开红包的一个低级错误，重新抓取了坐标点，优化了代码逻辑，现在更不容易卡死。
收火车重启策略更改为每次收完都重启，无论是否有不需要的低成色货物。

3.1

1. 自动适配分辨率，已测试720* 1280， 1080* 1920
2. 实现自动收货，
收货方式为当出现不想要的货物时，本轮收完所需货物立即重启游戏。
只收橙色，只收橙紫，全收三种模式可选。把收货函数里不需要的两种模式注释掉即可。

3. 自动升级政策中心
实现优先升级指定政策。
指定政策优先，可依次指定全部5个，也可以指定最前面的1个或者2个。如果指定政策已满，自动按顺序升级其他政策。

4. 自动升级指定建筑，默认为右上角9号，程序内id=8，可改为任意建筑，以及多个建筑。
5. 自动收钱，执行间隔为2分钟，可通过更改iter值改变。

3.0 

1. 新增一键换装
指定收货配置和平时配置，即可一件换装收货，收完又自动换回来。
2. 新增分辨率适配
3. 新增指定政策升级

2.2 

修复了进去政策中心后立刻退出的BUG。

2.0 
云手机版

1. 目前只能通过固定位置更换，因此只适用于右上角零件厂的情形。
一键换装还在调试中，手头没有趁手的工具，还有些建筑识别错误。
2. 修复了进入政策中心卡死的BUG。

二. 只收货不换建筑3.6

3.6 修复了政策中心升错政策的bug,感谢NGA水友 tannium 。

3.5

修复了政策中心和更换建筑时翻页的死循环
修复了政策中心的一处坐标错误

3.4
怎么说呢，又一次修复了进入政策中心卡死的BUG

3.3

进一步延长了重启游戏的延时到15秒，以避免意外的卡顿造成在登陆页面点击的众多BUG，未来将进一步优化防卡顿逻辑。


3.2

新增指定政策优先升级，重新抓取了坐标点，优化了代码逻辑，现在更不容易卡死。
收火车重启策略更改为每次收完都重启，无论是否有不需要的低成色货物。

3.0

新增指定政策升级

2.2

修复了进去政策中心后立刻退出的BUG。
修复了一个导致大面积收货故障的错误。

2.1

1. 重构了代码，能够自动适配各种分辨率，横版除外。已测试720* 1280， 1080* 1920。
2. 修复了进入政策中心卡死的BUG。

三. 自动收红包

2.1
修复了开红包的一个低级错误

2.0
新增分辨率适配
******************************************************
备注:
1. 当出现杀进程后，重复登录卡死，请适当延长重启后等待时间，如果机器比较卡，请进一步延长到10秒
2. 如果登录出现故障，请确认手动重复登录授权可用。
3. 如果杀进程后没能重启游戏，请检查按键精灵和游戏是否有唤醒权限以及后台弹出权限。
