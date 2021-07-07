﻿## 0 前言说明
1. **下载说明：由于可执行文件比较大，如有需要请到网盘下载。**
2. **网店地址：https://shop244026315.taobao.com/**
3. **联系方式：QQ：517216493  微信：feiyangqingyun  QQ好友满了推荐加微信**
4. **视频相关作品体验地址：[https://pan.baidu.com/s/1d7TH_GEYl5nOecuNlWJJ7g](https://pan.baidu.com/s/1d7TH_GEYl5nOecuNlWJJ7g) 提取码：01jf**
5. **其他相关作品体验地址：[https://pan.baidu.com/s/1ZxG-oyUKe286LPMPxOrO2A](https://pan.baidu.com/s/1ZxG-oyUKe286LPMPxOrO2A) 提取码：o05q**

## 1 自定义控件大全
### 1.1 控件介绍
1. 超过188个精美控件并持续不断迭代更新升级，种类超多，控件类型极其丰富。
2. 涵盖了各种仪表盘、进度条、进度球、指南针、曲线图、标尺、温度计、导航条、导航栏，flatui、高亮按钮、滑动选择器、农历、广告轮播、饼状图、环形图、时间轴、拓展控件、增强控件等。
3. 每个类都是独立的一个.h头文件和.cpp实现文件组成，零耦合，不依赖其他文件，方便单个控件独立出来以源码形式集成到项目中，方便直观。
4. 控件数量远超其他第三方控件库比如qwt集成的控件数量，使用方式也比其简单友好零耦合。
5. 支持任意Qt版本，亲测Qt4.6到Qt5.15的所有版本，全部纯Qt编写，QWidget+QPainter绘制。
6. 支持任意编译器，包括但不限于mingw、msvc、gcc、clang等编译器。
7. 支持任意操作系统，包括但不限于windows、linux、mac、android、uos、银河麒麟、各种国产linux、嵌入式linux、树莓派、香橙派、全志H3等。
8. 支持编译生成设计师插件，可直接集成到QtCreator的控件栏中，和自带的控件一样使用，大部分效果只要设置几个属性即可，极为方便。
9. 支持编译生成独立的非插件形式的动态库文件，体积小，比如嵌入式linux不支持designer只需要动态库的形式。
10. 每个控件都有一个单独的完整的使用demo，方便参考学习单个控件使用，非常适合初学者。
11. 提供一个所有控件使用的集成的example，方便快速查看所有控件的效果。
12. 支持直接源码集成到example的方式，方便编译到安卓，for web套件等。
13. 支持编译成wasm文件，直接网页运行，可以在谷歌、火狐、edge等浏览器运行，原生性能。
14. 每个控件的源代码都有详细中文注释，都按照统一设计规范编写，方便学习自定义控件的编写。
15. 每个控件都内置默认配色，demo对应的配色都非常精美。
16. 部分控件提供多种样式风格选择，多种指示器样式选择。
17. 所有控件自适应布局和窗体拉伸变化，自动缩放。
18. 配套额外的自定义控件属性设计器，类似组态设计器，纯中文属性名称，支持拖曳设计，所见即所得，支持导入导出xml格式。
19. 集成fontawesome图形字体+阿里巴巴iconfont收藏的几百个图形字体，享受图形字体带来的乐趣。
20. 所有控件最后生成一个dll动态库文件，可以直接集成到qtcreator中拖曳设计使用。
21. 控件源码全部分门别类存放，pri模块形式集成，提供控件对照表快速查找对应控件和说明。

### 1.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_quc/000.gif)

## 2 输入法
### 2.1 输入法V2018
1. 未采用Qt系统层输入法框架，独创输入切换机制。
2. 纯QWidget编写，支持任何目标平台（亲测windows、linux、嵌入式linux等），支持任意Qt版本（亲测Qt4.6.0到Qt5.11.2），支持任意编译器（亲测mingw、gcc、msvc等），支持任意控件输入包括网页中的输入控件。
3. 调用极为方便，pri文件调用形式，只要改成文件包含即可，例如pro文件中写 include($$PWD/inputnew/inputnew.pri)。
4. 界面清晰简洁，UI美观友好，非常适合触摸设备。
5. 支持实体键盘输入+鼠标单击输入+触摸输入。
6. Qt程序嵌入的浏览器中的网页中的文本框等控件的输入。
7. 迷你模式，界面大小随意设置，采用布局自使用任何分辨率。
8. 纯数字键盘模式，自由控制弹出完整输入法面板和数字键盘面板，只需要对控件设置属性即可。例如ui->txt->setProperty("flag", "number");
9. 控制需要显示输入法和不需要显示输入法，当某些控件不需要弹出输入法，只需要对应不需要弹出输入法的控件设置属性noinput为真即可。例如ui->txt->setProperty("noinput", true);
10. 自适应屏幕大小，输入法弹出位置为控件底部时，当超过桌面右边或者底部时，自动调整位置。
11. 实现了长按超过500毫秒重复执行按下的键的功能。例如长按退格键，不断删除。
12. shift键切换输入法，esc键隐藏输入法，空格选中第一个汉字，回车选中输入的拼音。和搜狗输入法处理一致。
13. 英文、中文、数字字母、大小写、特殊字符自由切换。
14. 支持单拼双拼词组输入，网上大部分只支持单个汉字输入。智能分页算法，可任意翻页查看汉字词组。
15. 默认自带5种皮肤颜色，可随意切换，用户也可用QSS自定义皮肤。
16. 字库文件可大可小，提供迷你版字库大小仅120KB，方便存储空间紧张的硬件，完整版字库25MB。
17. 可选谷歌内核的输入法引擎，字库文件1MB，不依赖数据库，资源占用低效率极高。支持模糊拼音，比如nh=你好。
18. 可选windows专有版本，支持外部程序输入，比如输入到记事本、QQ聊天窗口等。
19. 整个输入法代码行数1000行左右，非常小，不会对程序增加大小造成负担。
20. 代码结构极为清晰，注释详细，非常容易阅读和理解，同时也可以自行修改拓展自定义的需求。

### 2.2 输入法V2019
1. 未采用Qt系统层输入法框架，独创输入切换机制。
2. 纯QWidget编写，支持任何目标平台（亲测windows、linux、嵌入式linux等），支持任意Qt版本（亲测Qt4.6.0到Qt5.13），支持任意编译器（亲测mingw、gcc、msvc等），支持任意控件输入包括网页中的输入控件。
3. 调用极为方便，pri文件调用形式，只要改成文件包含即可，例如pro文件中写 include($$PWD/input2019/input2019.pri)。
4. 界面清晰简洁，UI美观友好，高仿IOS输入法，非常适合触摸设备。
5. 顶部滑动选词+弹出汉字面板选词，支持滑动。
6. 具有记忆功能，之前选中过的词语首先显示，支持单个拼音多个汉字，自动调整优先级。
7. 具有造词功能，可以直接打开文件文件写入自定义词组，最高级别显示。
8. 支持数字小键盘，可选是弹出全键盘的数字面板还是小键盘。
9. 多版面字符页面，可以自行拓展各种字符展示，可用于多语言输入。
10. 支持Qt程序嵌入的浏览器中的网页中的文本框等控件的输入。
11. 界面大小随意设置，采用布局自使用任何分辨率。
12. 属性控制数字输入，例如需要文本框默认弹出的是数字则设置代码 ui->txt->setProperty("flag", "number");
13. 自由控制需要显示输入法和不需要显示输入法，当某些控件不需要弹出输入法，只需要对应不需要弹出输入法的控件设置属性noinput为真即可。例如ui->txt->setProperty("noinput", true);
14. 界面自适应屏幕大小，输入法弹出位置为控件底部时，当超过桌面右边或者底部时，自动调整位置。
15. 实现了长按超过500毫秒重复执行按下的键的功能。例如长按退格键，不断删除。
16. 英文、中文、数字字母、大小写、特殊字符自由切换。
17. 支持单拼、全拼、模糊拼音输入，智能分页算法，可任意翻页查看汉字词组。
18. 默认自带5种皮肤颜色，可随意切换，用户也可用QSS自定义皮肤。
19. 谷歌内核的输入法引擎，品质保证，字库文件1MB，不依赖数据库，资源占用低效率极高。支持模糊拼音，比如nh=你好。
20. 可选windows专有版本，支持外部程序输入，比如输入到记事本、QQ聊天窗口等。
21. 整个输入法代码行数1000行左右，非常小，不会对程序增加大小造成负担。
22. 代码结构极为清晰，注释详细，非常容易阅读和理解，同时也可以自行修改拓展自定义的需求。

### 2.3 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_input/input2018.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_input/input2019.gif)

## 3 气体安全管理系统
### 3.1 功能特点
1. 采集数据端口，支持串口端口+网络端口，串口支持自由设置串口号+波特率，网络支持自由设置IP地址+通讯端口，每个端口支持采集周期，默认1秒钟一个地址，支持设置通讯超时次数，默认3次，支持最大重连时间，用于重新读取离线的设备。
2. 控制器信息，能够添加控制器名称，选择控制器地址+控制器型号，设置该控制器下面的探测器数量。
3. 探测器信息，能够添加位号，可自由选择探测器型号，气体种类，气体符号，高报值，低报值，缓冲值，清零值，是否启用，报警声音，背景地图，存储周期，数值换算小数点位数，报警延时时间，报警的类型（HH,LL,HL）等。
4. 控制器型号+探测器型号+气体种类+气体符号，均可自由配置。
5. 地图支持导入和删除，所有的探测器对应地图位置可自由拖动保存。
6. 端口信息+控制器信息+探测器信息，支持导入导出+导出到excel+打印。
7. 运行记录+报警记录+用户记录，支持多条件组合查询，比如时间段+控制器+探测器等，所有记录支持导出到excel+打印。
8. 导出到excel的记录支持所有excel+wps等表格文件版本，不依赖excel等软件。
9. 可删除指定时间范围内的数据，支持自动清理早期数据，设置最大保存记录数。
10. 支持报警短信转发，支持多个接收手机号码，可设定发送间隔，比如即时发送或者6个小时发送一次所有的报警信息，短信内容过长，自动拆分多条短信。
11. 支持报警邮件转发，支持多个接收邮箱，可设定发送间隔，比如即时发送或者6个小时发送一次所有的报警信息，支持附件发送。
12. 高报颜色+低报颜色+正常颜色+0值颜色+曲线背景+曲线颜色等，都可以自由选择。
13. 软件的中文标题+英文标题+logo路径+版权所有都可以自由设置。
14. 提供开关设置开机运行+报警声音+自动登录+记住密码等。
15. 报警声音可设置播放次数，界面提供17种皮肤文件选择。
16. 支持云端数据同步，可设置云端数据库的信息，比如数据库名称，用户名+密码等。
17. 支持网络转发和网络接收，网络接收开启后，软件从udp接收数据进行解析。网络转发支持多个目标IP，这样就实现了本地采集的软件，自由将数据转到客户端，随时查看探测器数据。
18. 自动记住用户最后停留的界面+其他信息，重启后自动应用。
19. 报警自动切换到对应的地图，探测器按钮闪烁。
20. 双击探测器图标，可以进行回控。
21. 支持用户权限管理，管理员+操作员两大类，用户登录+用户退出，可以记住密码和自动登录，超过三次报错提示并关闭程序。
22. 支持四种监控模式，设备面板监控+地图监控+表格数据监控+曲线数据监控，可自由切换，四种同步应用。
23. 支持报警继电器联动，一个位号可以跨串口联动多个模块和继电器号，支持多对多。
24. 本地数据存储支持sqlite+mysql，支持远程数据同步到云端数据库。自动重连。
25. 本地设备采集到的数据实时上传到云端，以便手机APP或者web等其他方式提取。
26. 支持两种数据源，一种是串口和网络通过协议采集设备数据，一种是数据库采集。数据库采集模式可以作为通用的系统使用。
27. 自带设备模拟工具，支持16个设备数据模拟，同时还带数据库数据模拟，以便在没有设备的时候测试数据。
28. 支持所有windows操作系统+linux操作系统和其他操作系统。

### 3.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_sams/sams.gif)

## 4 可视化大屏电子看板系统
### 4.1 功能特点
1. 采用分层设计，整体总共分三级界面，一级界面是整体布局，二级界面是单个功能模块，三级界面是单个控件。
2. 子控件包括饼图+圆环图+曲线图+柱状图+柱状分组图+横向柱状图+横向柱状分组图+合格率控件+百分比控件+进度控件+设备状态面板+表格数据+地图控件+视频控件等。
3. 二级界面可以自由拖动悬浮，支持最小化最大化关闭，响应双击自定义标题栏。
4. 数据源支持模拟数据（默认）、数据库采集、串口通信（需定制）、网络通信（需定制）、网络请求等，可自由设定每个子界面的采集间隔即数据刷新频率。
5. 采用纯QWidget编写，亲测Qt4.6到Qt5.15任意版本，理论上支持后续其他Qt版本，亲测win+linux+mac+uos+kylin等系统，效果完美，同时还支持嵌入式linux比如树莓派、香橙派、全志、imx6等。
6. 同时集成了自定义控件+qchart饼图+echart地图功能。
7. 内置多套配色风格样式（紫色、蓝色、深蓝、黑色），默认紫色，支持任何分辨率。
8. 可设置标题+目标分辨率+布局方案，启动立即应用。
9. 可设置主背景颜色+面板颜色+十字线游标颜色。
10. 可设置多条曲线颜色，没有设置颜色的情况下内置15套精美颜色随机应用。
11. 可设置标题栏背景颜色+文字颜色。
12. 可设置曲线图表背景颜色+文字颜色+网格颜色。
13. 可设置正常颜色+警戒颜色+报警颜色+禁用颜色+百分比进度颜色。
14. 可分别设置各种字体大小，比如全局+软件名称+标题栏+子标题栏+加粗标签等。
15. 可设置标题栏高度+表头高度+行高度。
16. 曲线支持游标+悬停高亮数据点和显示值，柱状图支持顶部（可设置顶端+上部+中间+底部）显示数据，全部自适应计算位置。
17. 主界面直接鼠标右键切换布局+配色方案+关闭开启某个二级窗体。
18. 自动记忆所有子窗口的大小和位置，下次启动立即应用。
19. 动态加载布局方案菜单，可以动态新建布局、恢复布局、保存布局、另存布局等，用户可以制造任意布局。
20. 二级窗体，双击从主窗体分离出来浮动，可以自由调整大小。再次双击标题栏最大化，再次双击还原，相当于子模块也可以全屏显示作为一个大屏，这样就可以一个大屏拓展出多个子大屏，放大查看子模块的数据详情。
21. 每个模块都可以自定义采集速度，如果是数据库采集会自动排队处理，后期还可以拓展每个子模块都独立的数据库采集。
22. 提供系统设置窗口进行整体的配置参数设置。
23. 提供精美炫酷的大屏地图模块，包括静态图片+闪烁效果+迁徙效果+世界地图+区域地图等，可指定点的经纬度坐标，识别单击响应，可以做地图跳转等，每个点都可以不同的颜色和提示信息，功能超牛逼！
24. 除了提供大屏系统外，还将每个模块都做了独立的模块示例界面，每个模块都可以独立学习使用，里面用到的控件也单独做了控件示例界面，方便学习每个控件如何使用，考虑着实周到！
25. 超级详细的开发和使用手册，其中包括详细的数据库说明、模块对照图、控件对照图、项目结构代码说明、使用方法等！

### 4.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_bigscreen/0.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_bigscreen/1.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_bigscreen/2.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_bigscreen/3.gif)


## 5 视频监控系统
### 5.1 软件模块
1. 视频监控模块，各种停靠小窗体子模块，包括设备列表、图文警情、窗口信息、云台控制、预置位、巡航设置、设备控制、悬浮地图、网页浏览等。
2. 视频回放模块，包括本地回放、远程回放、设备播放、图片回放、视频上传等。
3. 电子地图模块，包括图片地图、在线地图、离线地图、路径规划等。
4. 日志查询模块，包括本地日志、设备日志等。
5. 系统设置模块，包括系统设置（基本设置、视频参数、数据库设置、地图配置、串口配置等）、录像机管理、摄像机管理、轮询配置、用户管理等。

### 5.2 基础功能
1. 支持各种视频流（rtsp、rtmp、http等）、视频文件（mp4、rmvb、avi等）、本地USB摄像机播放。
2. 支持多画面切换，包括1、4、6、8、9、13、16、25、36、64画面切换。
3. 支持全屏切换，多种切换方式包括鼠标右键菜单、工具栏按钮、快捷键（alt+enter全屏，esc退出全屏）。
4. 支持视频轮询，包括1、4、9、16画面轮询，可设置轮询分组（轮询预案）、轮询间隔、码流类型等。
5. 支持onvif协议，包括设备搜索、云台控制、设备控制（图片参数、校对时间、系统重启，抓拍图片等）。
6. 支持权限管理，不同的用户可以对应不同的模块权限，比如删除日志、关闭系统等。
7. 数据库支持多种，包括sqlite、mysql、sqlserver、postgresql、oracle、人大金仓等。
8. 本地USB摄像机支持设置分辨率、帧率等参数。
9. 所有停靠模块都自动生成对应的菜单用来控制显示和隐藏，在标题栏右键可以弹出。
10. 支持显示所有模块、隐藏所有模块、复位普通布局、复位全屏布局。
11. 双击设备弹出实时预览视频，支持图片地图、在线地图、离线地图等。
12. 摄像机节点拖曳到对应窗体播放视频，同时支持拖曳本地文件直接播放。
13. 删除视频支持鼠标右键删除、悬浮条关闭删除、拖曳到视频监控面板外删除等多种方式。
14. 图片地图上设备按钮可自由拖动，自动保存位置信息。百度地图上可以鼠标单击获取经纬度信息，用来更新设备位置。
15. 视频监控面板窗体中任意通道支持拖曳交换，瞬间响应。
16. 封装了百度地图，视图切换，运动轨迹，设备点位，鼠标按下获取经纬度等。
17. 双击节点、拖曳节点、拖曳窗体交换位置等操作，均自动更新保存最后的播放地址，下次软件打开自动应用。
18. 右下角音量条控件，失去焦点自动隐藏，音量条带静音图标。
19. 支持视频截图，可指定单个或者对所有通道截图，底部小工具栏也有截图按钮。
20. 支持超时自动隐藏鼠标指针、自动全屏机制。
21. 支持onvif云台控制，可上下左右移动云台摄像机，包括复位和焦距调整等。
22. 支持任意onvif摄像机，包括但不限于海康、大华、宇视、天地伟业、华为等。
23. 可保存视频，可选定时存储或者单文件存储，可选存储间隔时间。
24. 可设置视频流通信方式tcp+udp，可设置视频解码是速度优先、质量优先、均衡等。
25. 可设置软件中文名称、英文名称、LOGO图标等。
26. 存储的视频文件支持导出到指定目录，支持批量上传到服务器。

### 5.3 特色功能
1. 主界面采用停靠窗体模式，各种组件以小模块的形式加入，可自定义任意模块加入。
2. 停靠模块可拖动任意位置嵌入和悬浮，支持最大化全屏，支持多屏幕。
3. 双重布局文件存储机制，正常模式、全屏模式都对应不同的布局方案，自动切换和保存，比如全屏模式可以突出几个模块透明显示在指定位置，更具科幻感现代化。
4. 原创onvif协议机制，采用底层协议解析（udp广播搜索+http请求执行命令）更轻量易懂易学习拓展，不依赖任何第三方组件比如gsoap。
5. 原创数据导入导出机制，跨平台不依赖任何组件，瞬间导出数据。
6. 内置多个原创组件，宇宙超值超级牛逼，包括数据导入导出组件（导出到xls、pdf、打印）、数据库组件（数据库管理线程、自动清理数据线程、万能分页、数据请求等）、地图组件、视频监控组件、文件多线程收发组件、onvif通信组件、通用浏览器内核组件等。
7. 自定义信息框+错误框+询问框+右下角提示框（包含多种格式）等。
8. 精美换肤，高达17套皮肤样式随意更换，所有样式全部统一，包括菜单等。
9. 视频控件悬浮条可以自行增加多个按钮，监控界面底部小工具栏也可自行增加按钮。
10. 双击摄像机节点自动播放视频，双击节点自动依次添加视频，会自动跳到下一个，双击父节点自动添加该节点下的所有视频。可选主码流、子码流。
11. 录像机管理、摄像机管理，可添加删除修改导入导出打印信息，立即应用新的设备信息生成树状列表，不需重启。
12. 可选多种内核自由切换，ffmpeg、vlc、mpv等，均可在pro中设置。推荐用ffmpeg，跨平台最多，默认提供好了linux和mac平台上编译好的库。
13. 支持硬解码，可设置硬解码类型（qsv、dxva2、d3d11va等）。
14. 默认采用opengl绘制视频，超低的CPU资源占用，支持yuyv和nv12两种格式绘制，很牛逼。
15. 高度可定制化，用户可以很方便的在此基础上衍生自己的功能，比如增加自定义模块，增加运行模式、机器人监控、无人机监控、挖掘机监控等。
16. 支持xp、win7、win10、linux、mac、各种国产系统（UOS、中标麒麟、银河麒麟等）、嵌入式linux等系统。
17. 注释完整，项目结构清晰，超级详细完整的使用开发手册，精确到每个代码文件的功能说明，不断持续迭代版本。

### 5.4 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_video_system/0.gif)

## 6 智能安防集中管理平台
### 6.1 功能特点
1. 同时集成了楼宇对讲、住户报警、门禁控制、公共报警、视频监控等模块。
2. 系统管理部分包括系统配置、对讲配置、住户配置、公共配置、监控配置、地图管理、视频联动、用户管理、区域管理。
3. 图形化的实时对讲、室内报警、门禁设备界面，非常大气美观。
4. 设备状态内置地图模式、面板模式两种方式展示，非常强大。
5. 楼宇对讲设备和报警设备都支持地图上拖曳到正确位置，保存立即应用。
6. 支持报警视频联动，设备报警对应弹出报警视频。
7. 各种设备信息支持添加、删除、修改、打印、导入、导出、查询等，支持多条件组合查询。
8. 各种日志信息支持多条件组合模糊查询，查询的记录可导出和打印。
9. 可直接在软件上授权发卡，支持多对多发卡，一个卡号可以发到多个门禁设备，支持通卡（卡号下发到所有设备），可连续自动制卡，自动选中下一个用户进行制卡。
10. 可直接远程读取选中设备的卡号集合信息，进行统一的管理。
11. 所有卡号支持本地备份，一旦远程设备更换，可以重新下发卡号信息。
12. 支持过期卡号自动清理，被清理的卡号可以查询，可以指定楼栋、单元、过期时间查询卡号。
13. 支持公共部位报警接入，默认DS7400主机，能够识别布防、撤防、报警等信息。
14. 视频监控默认支持16通道显示，可切换到4通道、6通道、8通道、9通道、13通道显示，支持全屏和轮询。
15. 首页背景图、左上角logo、右上角项目名称可自定义，支持恢复出厂设置。
16. 亿级别本地海量数据存储，自动清空早期数据，永远保持最新的数据记录。
17. 每个模块都有开关可以后台自由控制启用或者禁用。
18. 集成了秘钥控制功能，可以控制设备数量以及运行时间。
19. 内置最牛逼的豪华版的输入法，高仿苹果电脑输入法，体验一级棒。
20. 纯Qt编写，支持任意Qt版本+任意编译器+任意系统，可运行在windws XP、win7、win8、win10、linux、mac OS、嵌入式linux等系统。

### 6.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_TB/0.jpg)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_TB/1.jpg)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_TB/2.jpg)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_TB/3.jpg)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_TB/4.jpg)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_TB/5.jpg)

## 7 视频监控内核
### 7.1 ffmpeg内核
1. 多线程实时播放视频流+本地视频+USB摄像头等。
2. 支持windows+linux+mac，支持ffmpeg3和ffmpeg4，支持32位和64位。
3. 多线程显示图像，不卡主界面。
4. 自动重连网络摄像头。
5. 可设置边框大小即偏移量和边框颜色。
6. 可设置是否绘制OSD标签即标签文本或图片和标签位置。
7. 可设置两种OSD位置和风格。
8. 可设置是否保存到文件以及文件名。
9. 可直接拖曳文件到ffmpegwidget控件播放。
10. 支持h265视频流+rtmp等常见视频流。
11. 可暂停播放和继续播放。
12. 支持存储单个视频文件和定时存储视频文件。
13. 自定义顶部悬浮条，发送单击信号通知，可设置是否启用。
14. 可设置画面拉伸填充或者等比例填充。
15. 可设置解码是速度优先、质量优先、均衡处理。
16. 可对视频进行截图（原始图片）和截屏。
17. 录像文件存储支持裸流和MP4文件。
18. 音视频完美同步，采用外部时钟同步策略。
19. 支持seek定位播放位置。
20. 支持在线网络音视频文件比如http开头mp4、mp3结尾的。
21. 可选句柄模式（GPU绘制）、回调模式（QPainter绘制）。
22. GPU绘制模式同时支持拉伸和等比例绘制。
23. 支持qsv、dxva2、d3d11va等硬解码。
24. 硬解码和GPU组合，超低CPU占用，支持64路视频。
25. 支持安卓和嵌入式linux，交叉编译即可。

### 7.2 vlc内核
1. 多线程实时播放rtsp视频流。
2. 支持windows+linux+mac。
3. 多线程显示图像，不卡主界面。
4. 自动重连网络摄像头。
5. 可设置边框大小即偏移量和边框颜色。
6. 可设置是否绘制OSD标签即标签文本或图片和标签位置。
7. 可设置两种OSD位置和风格。
8. 可设置是否保存到文件以及文件名。
9. 可播放本地视频文件，支持设置帧率。
10. 支持h265视频流+rtmp等常见视频流。
11. 可暂停播放和继续播放。
12. 支持回调模式和句柄两种模式。
13. 自动将当前播放位置和音量大小是否静音以信号发出去。
14. 提供接口设置播放位置和音量及设置静音。
15. 支持定时存储视频文件。
16. 支持外部拖曳文件+拖曳节点数据进行播放。
17. 自定义顶部悬浮条，发送单击信号通知，可设置是否启用。

### 7.3 mpv内核
1. 多线程实时播放视频流+本地视频等。
2. 支持windows+linux+mac。
3. 多线程显示图像，不卡主界面。
4. 自动重连网络摄像头。
5. 可设置是否保存到文件以及文件名。
6. 可直接拖曳文件到mpvwidget控件播放。
7. 支持h265视频流+rtmp等常见视频流。
8. 可暂停播放和继续播放。
9. 支持存储单个视频文件和定时存储视频文件。
10. 自定义顶部悬浮条，发送单击信号通知，可设置是否启用。
11. 可设置画面拉伸填充或者等比例填充。
12. 可对视频进行截图（原始图片）和截屏。
13. 录像文件存储MP4文件。
14. 支持qsv、dxva2、d3d11va等硬解码。

### 7.4 海康内核
1. 支持播放视频流和本地MP4文件。
2. 支持句柄和回调两种模式。
3. 多线程显示图像，不卡主界面。
4. 自动重连网络摄像头。
5. 可设置边框大小即偏移量和边框颜色。
6. 可设置是否绘制OSD标签即标签文本或图片和标签位置。
7. 可设置两种OSD位置和风格。
8. 可设置是否保存到文件以及文件名。
9. 可直接拖曳文件到haikangwidget控件播放。
10. 支持h264/h265视频流。
11. 可暂停播放和继续播放。
12. 支持存储单个视频文件和定时存储视频文件。
13. 自定义顶部悬浮条，发送单击信号通知，可设置是否启用。
14. 可设置画面拉伸填充或者等比例填充。
15. 可设置解码是速度优先、质量优先、均衡处理。
16. 可对视频进行截图（原始图片）和截屏（视频窗体）。
17. 录像文件存储为MP4文件。
18. 支持焦距控制、云台控制。
19. 可定制功能。

### 7.5 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_video_ffmpeg/video_ffmpeg1.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_video_vlc/video_vlc1.gif)

## 8 皮肤生成器+UIDemo
### 8.1 功能特点
1. 自带17套精美皮肤样式，其中包括黑色、灰色、扁平等。
2. 皮肤生成器只需要简单几步就可以生成一套自定义的皮肤。
3. 自带了26种uidemo，非常漂亮美观，涵盖了主界面布局、菜单切换等各种效果，总有一款适合你。
4. 所有代码和demo注释都非常详细整齐整洁，非常适合初学者学习。
5. uidemo由简入难，可以一步步学习下去，从入门到熟悉。
6. uidemo从常规的客户端到app端到触摸端等都有，既有鼠标操作的也有触摸操作的。
7. 皮肤中的qss样式表内容，覆盖了几乎所有的控件，非常适合学习每个控件的qss样式如何设置，而且分门别类非常清晰。
8. 自带的quiwidget类，集大成之所长，超级牛逼，内置了无边框的消息框、错误框、询问框、右下角信息框、输入框、日期范围选择框等，支持倒计时关闭，集成图形字体设置方法及根据指定文字获取图片，集成CRC校验、获取应用程序文件名、文件路径、设置窗体居中显示、设置翻译文件、设置编码、设置延时、设置系统时间等各种静态方法，保你满意。
9. 支持任意Qt版本+任意编译器+任意系统，可运行在win、linux、mac OS、嵌入式linux等各种系统上。

### 8.2 使用方法
1. 单击另存为按钮，可以将当前看到的界面的样式导出到一个样式表文件，包含自动生成的图片资源。
2. 右上角风格下拉菜单，可以切换17套皮肤，切换完成以后会自动应用。
3. 支持直接在右侧样式表编辑栏内直接修改样式表内容，修改完成立即应用。
4. 从左侧选择字体颜色+面板背景+渐变颜色等，只要选择8种颜色，就可以生成一套自己的皮肤。
5. 皮肤生成器只是用来生成统一风格的样式表，比如按钮+文本框+菜单等控件的风格，而不是生成ui界面文件。
6. 对应的uidemo是样式表+ui布局的整体综合应用，可以自行修改成自己想要的布局。
7. QChar图形字体的对照表在 图形字体对照表.png。

### 8.3 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_uidemo/qui.gif)

## 9 Onvif搜索和云台控制工具
### 9.1 功能特点
1. 广播搜索设备，支持IPC和NVR，依次返回，可选择不同的网卡IP。
2. 依次获取Onvif地址、Media地址、Profile文件、Rtsp地址。
3. 可对指定的Profile获取视频流Rtsp地址，比如主码流子码流地址。
4. 可对每个设备设置Onvif用户信息，用于认证获取详细信息。
5. 可实时预览摄像机图像。
6. 支持云台控制，可上下左右调节云台，支持绝对移动和相对移动，可放到和缩小图像远近。
7. 支持Qt4和Qt5任意Qt版本，亲测Qt4.7.0到Qt5.14.2。
8. 支持任意编译器，亲测mingw、msvc、gcc、clang。
9. 支持任意操作系统，亲测xp、win7、win10、android、linux、嵌入式linux、树莓派全志H3等。
10. 支持任意Onvif摄像机和NVR，亲测海康、大华、宇视、华为、海思芯片内核等，可定制开发。
11. 支持对指定IP地址及onvif地址进行单播搜索，比如跨网段情况下非常有用。
12. 支持指定过滤条件过滤搜索设备。
13. 支持搜索间隔设置，保证所有设备搜索回来，在大量设备现场很有用。
14. 可对图片参数（亮度、色彩度、饱和度）进行设置。
15. 支持NTP校时和时间同步设置。
16. 纯Qt编写，超级小巧轻量，总共约2000行代码，不依赖任何第三方的库和组件，跨平台。
17. 封装好了通用的数据发送和接收解析的函数，可以非常方便的自行拓展其他Onvif处理。
18. 工具上提供了收发数据文本框，显示收发的数据，方便查看和分析。
19. 支持所有Onvif设备，代码工整，接口友好，直接引入pri即可使用。

### 9.2 主要功能
1. 搜索设备，获取设备的信息比如厂家、型号等。
2. 获取设备的多个配置文件信息profile。
3. 获取对应配置文件的视频流地址rtsp，以及分辨率等参数。
4. 云台控制，上下左右移动，焦距放大缩小，相对和绝对移动。
5. 获取预置位信息，触发预置位。
6. 订阅事件，接收设备的各种消息尤其是报警事件比如IO口的报警。
7. 抓图，获取设备当前的图片。
8. 获取、创建、删除用户信息。
9. 获取和设备网络配置信息比如IP地址等。
10. 获取和设置NTP时间同步以及设置设备时间。
11. 获取和设置视频参数和图片参数（亮度、色彩、饱和度）。
12. 重启设备。

### 9.3 处理流程
1. 绑定组播IP（239.255.255.250）和端口（3702），发送固定的xml格式的数据搜索设备。
2. 接收到的xml格式的数据解析，得到设备的Onvif地址。
3. 对Onvif地址发送对应的数据，收到数据取出对应的节点数据。
4. 请求Onvif地址获取Media地址和Ptz地址，Media地址用来获取详细的配置文件，Ptz地址用来云台控制。
5. ptz控制是对Ptz地址发送对应的数据即可。
6. 设置了用户认证的需要组织用户token信息一块发送，每次都需要作鉴权处理。
7. 接收到的数据不是标准的xml数据，没法按照正常的节点解析来处理，只能用QXmlQuery来做。
8. 每个厂家设备返回的数据未必完全一致，基本上都不一致，需要进行模糊查找节点值。
9. 特意采用底层协议解析，因为soap太臃肿函数名称太另类，特意做的轻量级的。
10. 两个必备工具，Onvif Device Manager 和 Onvif Device Test Tool。

### 9.4 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_video_onvif/video_onvif.gif)

## 10 控件属性设计器
### 10.1 功能特点
1. 自动加载插件文件中的所有控件生成列表，默认自带的控件超过120个。
2. 拖曳到画布自动生成对应的控件，所见即所得。
3. 右侧中文属性栏，改变对应的属性立即应用到对应选中控件，直观简洁，非常适合小白使用。
4. 独创属性栏文字翻译映射机制，效率极高，可以非常方便拓展其他语言的属性栏。
5. 所有控件的属性自动提取并显示在右侧属性栏，包括枚举值下拉框等。
6. 支持手动选择插件文件，外部导入插件文件。
7. 可以将当前画布的所有控件配置信息导出到xml文件。
8. 可以手动选择xml文件打开控件布局，自动根据xml文件加载控件。
9. 可拉动滑动条、勾选模拟数据复选框、文本框输入，三种方式来生成数据应用所有控件。
10. 控件支持八个方位拉动调整大小，自适应任意分辨率，可键盘上下左右微调位置。
11. 打通了串口采集、网络采集、数据库采集三种方式设置数据。
12. 代码极其精简，注释非常详细，可以作为组态的雏形，自行拓展更多的功能。
13. 纯Qt编写，支持任意Qt版本+任意编译器+任意系统。

### 10.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_property/完整视频.gif)

## 11 自定义曲线图柱状图
### 11.1 功能特点
1. 可设置X轴Y轴范围值。
2. 可设置背景颜色+文本颜色+网格颜色。
3. 可设置三条曲线颜色+颜色集合。
4. 可设置是否显示定位十字线,可分别设置横向和纵向。
5. 可设置十字线的宽度和颜色。
6. 可设置是否显示数据点以及数据点的大小。
7. 可设置是否填充背景形成面积图。
8. 可设置模式-拖动+缩放等。
9. 可设置坐标轴间距+第二坐标系可见。
10. 提供接口setDataLine直接设置曲线,支持多条。
11. 提供接口setDataBar直接设置柱状图,支持多条形成堆积图。
12. 提供接口setLabs设置文本标签替代key,包括X轴和Y轴。
13. 提供清空数据+重绘图表+外部获取QCustomPlot对象,这样就可以进行更加详细的参数设置。
14. 提供函数start+stop来模拟正弦曲线。
15. 可设置柱状图的值的位置+精确度+颜色。
16. 支持鼠标移动到数据点高亮显示数据点以及显示数据提示信息。
17. 可设置提示信息位置 自动处理+顶部+右上角+右侧+右下角+底部+左下角+左侧+左上角。
18. 可设置是否校验数据产生不同的背景颜色,比如柱状图的每根柱子都可以根据数据生成不同背景颜色。
19. 可设置是否显示图例+图例位置+图例行数以及图例单行显示。
20. 支持多条曲线+柱状图+柱状分组图+横向柱状图+横向分组图+柱状堆积图。
21. 内置15套精美颜色,自动取颜色集合的颜色,省去配色的烦恼。
22. 每条柱状图都可以设置不同的颜色,分组柱状图可以设置颜色交替。
23. Y轴数值支持百分比显示,可拓展成其他格式。
24. 内置平滑曲线算法,支持平滑曲线绘制,传入点集合即可。
25. 同时支持 QCustomPlot 1.0 和 QCustomPlot 2.0。
26. 支持Qt4-Qt5任意Qt版本,支持任意编译器+任意操作系统。

### 11.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_customplot/customplot.gif)

## 12 数据导入导出(xls/pdf)及打印示例
### 12.1 功能特点
1. 原创导出数据机制，不依赖任何office组件或者操作系统等第三方库，尤其是支持嵌入式linux。
2. 10万行数据9个字段只需要2秒钟完成。
3. 只需要四个步骤即可开始急速导出大量数据到Excel。
4. 同时提供直接写入数据接口和多线程写入数据接口，不卡主界面。
5. 可设置标题、副标题、表名。
6. 可设置字段名称、列宽度。
7. 可设置是否启用校验过滤数据、校验的列、校验规则、校验值，符合规则的特殊颜色显示。
8. 可设置随机背景颜色及需要随机背景色的列集合。
9. 支持分组输出数据，比如按照设备分组输出数据，方便查看。
10. 可自定义行内容分隔符。
11. 可追加数据形式写入数据，建议每次追加的数据小于10000条。
12. 灵活性超高，可自由更改源码设置对齐方式、文字颜色、背景颜色等。
13. 支持任意excel表格软件，包括但不限于excel2003/2007/2010/2013/2017/wps/openoffice等。
14. 除了提供导出到Excel类以外，还提供导出到Pdf文件以及打印数据的类。
15. 注释完善，详细完整的使用demo，支持QTableWidget、QTableView、数据库三种数据源。
16. 纯Qt编写，支持任意Qt版本+任意编译器+任意系统。

### 12.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_dataout/dataout.gif)

## 13 数据库集成应用通用功能
### 13.1 功能特点
1. 同时支持多种数据库比如odbc、sqlite、mysql、postgresql、sqlserver、oracle、人大金仓等。
2. 一个数据库类即可管理本地数据库通信，也支持远程数据库通信等。
3. 数据库线程支持执行各种sql语句，包括单条和批量。
4. 组件中的所有类打印信息、错误信息、执行结果都信号发出去。
5. 集成数据库通用翻页类（负责具体处理逻辑），搭配分页导航控件（负责外观），形成超级牛逼的翻页控件。
6. 集成数据库自动清理类，设定最大记录数后台自动清理早期数据。
7. 集成自定义委托类，支持复选框、文本框、下拉框、日期框、微调框、进度条等。
8. 同时支持Qt4-Qt6，亲测Qt4.6到Qt6.1任意版本，任意系统和编译器。
9. 本组件无故障 360天7乘24小时 运行在至少上万个现场，商业级别品质保证。
10. 每个类都对应完整详细的使用示例，注释详细，非常适合阅读学习。
11. 可以作为独立的程序运行，比如自动清理早期数据，同步数据到云端。
12. 全部线程处理，不卡界面，自动重连数据库。
13. 普通测试情况，sqlite数据库，数据库发生器每秒钟插入1000条记录约0.003秒钟，同时自动清理数据类每秒钟删除1000条记录约0.13秒，不同线程互不干扰。

### 13.2 数据库通信管理线程类
1. 可设置数据库类型，支持多种数据库类型。
2. 数据库类型包括但不限于odbc、sqlite、mysql、postgresql、sqlserver、oracle、人大金仓等。
3. 可设置数据库连接信息包括主机地址、用户信息等。
4. 具有自动重连机制，可设置是否检查连接以及检查间隔。
5. 支持单条sql语句队列，一般用于查询返回数据，每次插入一条执行一条。
6. 支持多条sql语句队列，一般用于远程提交数据，每次插入一条执行多条。
7. 支持批量sql语句队列，一般用于批量更新数据，每次插入多条执行多条。
8. 可设置队列最大数量，限定排队处理的sql语句集合。
9. 通过信号发出 打印信息、错误信息、查询结果。

### 13.3 数据库通用翻页类
1. 可设置每页多少行记录，自动按照设定的值进行分页。
2. 可设置要查询的表名、字段集合、条件语句、排序语句。
3. 可设置第一页、上一页、下一页、末一页、翻页按钮。
4. 可设置当前页、总页数、总记录数、每页记录数、查询用时标签页。
5. 多线程查询总记录数，数据量巨大时候不会卡主界面。
6. 建议条件字段用整型类型的主键，速度极快。
7. 提供查询结果返回信号，包括当前页、总页数、总记录数、查询用时等信息。
8. 可设置所有列或者某一列对齐样式例如居中或者右对齐。
9. 可增加列用于标识该条记录，设定列的位置、标题、宽度。
10. 提供函数直接执行第一页、上一页、下一页、末一页。
11. 提供函数直接跳转到指定页。
12. 根据是否第一页、末一页自动禁用对应的按钮。
13. 本控件是翻页功能类，和翻页控件navpage完美搭配，形成超级牛逼的翻页控件。

### 13.4 分页导航控件
1. 可设置页码按钮的个数。
2. 可设置字体大小。
3. 可设置边框圆角角度、大小、颜色。
4. 可设置正常状态背景颜色、文字颜色。
5. 可识别悬停状态背景颜色、文字颜色。
6. 可设置按下状态背景颜色、文字颜色。
7. 可设置选中状态背景颜色、文字颜色。
8. 可设置导航位置居中对齐、左对齐、右对齐。
9. 可设置是否显示提示标签控件。
10. 自动计算总页码数显示隐藏多余按钮。
11. 自动计算切换页码导航。
12. 和分页导航功能类无缝对接完美融合。

### 13.5 自动清理数据线程类
1. 可设置要清理的对应数据库连接名称和表名。
2. 可设置条件字段。
3. 可设置排序字段。
4. 可设置最大保留的记录数。
5. 可设置执行自动清理的间隔。
6. 后期支持多个数据库和多个表。
7. 建议条件字段用数字类型的主键，速度极快。
8. 增加统计用字段名称设置。
9. 增加自动清理文件夹，超过大小自动删除文件夹中早期文件。

### 13.6 自定义委托全家桶
1. 可设置多种委托类型，例如复选框、文本框、下拉框、日期框、微调框、进度条等。
2. 可设置是否密文显示，一般用于文本框。
3. 可设置是否允许编辑，一般用于下拉框。
4. 可设置是否禁用，一般用来禁用某列。
5. 可设置数据集合，比如下拉框数据集合。
6. 提供值变化信号，比方说下拉框值改动触发。
7. 可设置数据校验自动产生不同的图标。
8. 支持设置校验列、校验规则、校验值、校验成功图标、校验失败图标、图标大小。
9. 可设置校验数据产生不同的背景颜色和文字颜色。
10. 校验规则支持 == > >= < <= != contains，非常丰富。
11. 复选框自动居中而不是左侧，切换选中状态发送对应的信号。
12. 可设置颜色委托，自动根据颜色值绘制背景颜色，自动设置最佳文本颜色。
13. 可设置按钮委托，自动根据值生成多个按钮，按钮按下发送对应的信号。
14. 当设置了委托列时自动绘制选中背景色和文字颜色。
15. 可设置关键字对照表绘制关键字比如原始数据是 0-禁用 1-启用。
16. 可设置复选框对应的映射选中不选中关键字。
17. 根据不同的委托类型绘制，可以依葫芦画瓢自行增加自己的委托。
18. 所有功能封装成1个类，核心代码不到500行，使用极其方便友好。

### 13.7 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_dbtool/dbtool.gif)

## 14 图片及视频TCP/UDP网络传输
### 14.1 功能特点
1. 多线程收发图片数据和解析图片数据，不卡主界面。
2. 同时支持TCP和UDP两种模式，封装了TCP模式以及UDP模式的客户端类和服务端类。
3. 图片传输客户端同时支持发送到多个服务端，可以作为一个教师机同屏发送到多个学生机的应用场景。
4. 同时支持多个客户端同时往服务端发送图片，服务端每个连接都会自动开辟线程收发和解析图片数据。
5. 自定义label控件信号槽机制绘制图片，不卡主界面。
6. 自带心跳机制判断离线，自动重连服务器，可设置超时时间。
7. 每个消息都有唯一的消息标识uuid，服务端收到以后会返回对应的uuid消息表示收到，客户端可以根据此返回消息判断服务端解析成功，不用再发，这样可以确保发出去的数据服务器接收到了并解析成功。
8. 每个消息都有唯一的图片标识flag，相当于ID号，根据此标识判断需要解析显示到哪个界面。
9. 图片以base64的字符串格式发送，接收端接收到base64字符串的图片数据解码后重新生成图片。
10. 所有数据的收发都有信号发出去，方便输出查看。
11. 都提供单例类，方便只有一个的时候直接使用无需new。
12. 采用自定义的xml协议，可以自由拓展其他属性字段比如带上图片内容等。

### 14.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_video_image/video_image1.gif)

## 15 百度地图综合应用（在线+离线+区域+下载）
### 15.1 省市区域地图封装类功能特点
1. 同时支持闪烁点图、迁徙图、区域地图、世界地图、仪表盘等。
2. 可以设置标题、提示信息、背景颜色、文字颜色、线条颜色、区域颜色等各种颜色。
3. 可设置城市的名称、值、经纬度 集合。
4. 可设置地图的放大倍数、是否允许鼠标滚轮缩放。
5. 内置世界地图、全国地图、省份地图、地区地图，可以精确到县，所有地图全部离线使用。
6. 内置了各省市json数据文件转js文件功能，如有数据更新自行转换即可，支持单个文件转换和一键转换所有文件。
7. 内置了从json文件或者js文件获取该区域的所有名称和经纬度信息集合的功能，可以通过该方法获取到信息用来显示。
8. 依赖浏览器组件显示地图，提供的demo支持webkit/webengine/miniblink/ie 多种方式加载网页。
9. 采用miniblink浏览器内核打通了Qt5.6及后续版本+mingw编译器缺少浏览器模块的遗憾，使得整个项目支持所有Qt版本，亲测4.7到5.15等任意版本。
10. 闪烁点迁徙图等设置的点支持单独设置颜色。
11. 提供接口直接获取点击的点相关信息，方便程序联动处理。
12. 拓展性极强，可以依葫芦画瓢自行增加各种精美的echarts组件，做出牛逼的效果。
13. 内置的仪表盘组件提供交互功能，demo演示中包含了对应的代码。
14. 函数接口友好和统一，使用简单方便，就一个类。
15. 支持任意Qt版本、任意系统、任意编译器。

### 15.2 百度地图封装类功能特点
1. 同时支持在线地图和离线地图两种模式。
2. 同时支持webkit内核、webengine内核、miniblink内核、IE内核。
3. 支持设置多个标注点，信息包括名称、地址、经纬度。
4. 可设置地图是否可单击、拖动、鼠标滚轮缩放。
5. 可设置协议版本、秘钥、主题样式、中心坐标、中心城市、地理编码位置等。
6. 可设置地图缩放比例和级别，缩略图、比例尺、路况信息等控件的可见。
7. 支持地图交互，比如鼠标按下获取对应位置的经纬度。
8. 支持查询路线，可设置起点位置、终点位置、路线模式、路线方式、路线方案（最少时间、最少换乘、最少步行、不乘地铁、最短距离、避开高速）。
9. 可显示点线面工具，可直接在地图上划线、点、矩形、圆形等。
10. 可设置行政区划，指定某个城市区域绘制图层，在线地图自动输出行政区划边界点集合到js文件给离线地图使用。
11. 可静态或者动态添加多个覆盖物。支持点、折线、多边形、矩形、圆形、弧线、点聚合等。
12. 提供函数接口处理经纬度解析成地址和地址解析成经纬度坐标。
13. 提供的demo直接可以单独选点执行对应的处理比如路线查询。
14. 可以拿到路线查询到的点坐标信息集合，比如用于机器人坐标导航等。
15. 封装了丰富的函数比如删除指定点和所有点，删除指定覆盖物和所有覆盖物等。
16. 标注点弹框信息可以自定义内容，标准html格式。
17. 标注点单击事件可选 0-不处理 1-自己弹框 2-发送信号。
18. 标注点可设置动画效果 0-不处理 1-跳动 2-坠落
19. 标注点可设置本地图片文件等。
20. 函数接口友好和统一，使用简单方便，就一个类。
21. 支持js动态交互添加点、删除点、清空点、重置点，不需要刷新页面。
22. 支持任意Qt版本、任意系统、任意编译器。

### 15.3 离线地图下载类功能特点
1. 多线程同步下载多级别瓦片地图，不卡界面。
2. 内置多个离线地图下载请求地址，自动随机选择一个发送请求。
3. 下载地图类型同时支持街道图和卫星图。
4. 自动计算可视区域或者行政区域的下载瓦片数量。
5. 下载的级别可以自定义范围和选择。
6. 每个瓦片下载完成都发送信号通知，参数包括下载用时。
7. 可设置下载最大超时时间，超过了则丢弃跳到下一个下载任务。
8. 实时显示下载进度，以及当前级别已经下载的瓦片数和总瓦片数。
9. 下载过程中可以停止下载，下载完成自动统计总用时。
10. 内置经纬度和屏幕坐标互相转换函数。
11. 目前支持百度地图，其他地图比如谷歌地图、腾讯地图、高德地图可以定制。
12. 函数接口友好和统一，使用简单方便，就一个类。
13. 支持任意Qt版本、任意系统、任意编译器。

### 15.4 省市轮廓下载类功能特点
1. 定时器排队下载省市轮廓图点坐标集合存储到JS文件。
2. 支持一个行政区域多个不规则区域下载。
3. 自动计算行政区域的下载轮廓数量。
4. 可精确选择省份、市区、县城，也可直接输入行政区域的名称。
5. 可以设置下载间隔、随时开始下载和停止下载。
6. 提供编辑边界功能，可以直接在地图上编辑好不规则区域的点集合，然后获取边界点集合数据，这个可以用来自己绘制区域拿到数据，比如某个乡镇甚至某个小区的行政区域数据，很牛逼。

### 15.5 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_map/map_echart_win.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_map/map_baidu_win1.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_map/map_baidu_win2.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_map/map_baidu_win3.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_map/map_baidu_win4.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_map/map_download_win.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_map/map_boundary_win.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_map/map_demo_win.gif)

## 16 网络请求客户端/服务器
### 16.1 功能特点
1. 支持多个客户端连接并发同时处理，
2. 可设置http请求是长连接还是短连接，默认长连接。
3. 支持多种回复数据格式，其中包括网页内容、json数据等。
4. 服务端示例中同时包含读取文件回复、读取数据库回复。
5. 支持8种配色方案（暗黑、灰黑、深绿、浅黄、深蓝、深黑、暗蓝、默认）。
6. 客户端可指定请求地址，服务端可指定网卡和端口进行监听。
7. 所有请求和连接都有计数，所有在线请求的IP和端口都显示在表格中。
8. 可自由拓展增加权限校验等，作为一个http请求服务器。
9. 代码框架整洁，注释完整，支持任意Qt版本、任意编译器、任意操作系统。

### 16.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_httpserver/httpserver.gif)

## 17 自定义委托全家桶
### 17.1 功能特点
1. 可设置多种委托类型，例如复选框/文本框/下拉框/日期框/微调框/进度条等。
2. 可设置是否密文显示，一般用于文本框。
3. 可设置是否允许编辑，一般用于下拉框。
4. 可设置是否禁用，一般用来禁用某列。
5. 可设置数据集合，比如下拉框数据集合。
6. 提供值变化信号，比方说下拉框值改动触发。
7. 可设置数据校验自动产生不同的图标。
8. 支持设置校验列/校验规则/校验值/校验成功图标/校验失败图标/图标大小。
9. 可设置校验数据产生不同的背景颜色和文字颜色。
10. 校验规则支持 == > >= < <= != contain，非常丰富。
11. 复选框自动居中而不是左侧，切换选中状态发送对应的信号。
12. 可设置颜色委托，自动根据颜色值绘制背景颜色，自动设置最佳文本颜色。
13. 可设置按钮委托，自动根据值生成多个按钮,按钮按下发送对应的信号。
14. 当设置了委托列时自动绘制选中背景色和文字颜色。
15. 可设置关键字对照表绘制关键字比如原始数据是 0-禁用 1-启用。
16. 可设置复选框对应的映射选中不选中关键字。
17. 根据不同的委托类型绘制，可以依葫芦画瓢自行增加自己的委托。
18. 所有功能封装成1个类不到500行代码，使用极其方便友好。

### 17.2 应用场景
1. 某个字段需要提供下拉框进行选择，下拉框可选是否允许编辑。
2. 某个字段需要提供密码框进行输入，密文显示字段值。
3. 某个字段需要提供日期框下拉选择日期时间。
4. 某个字段需要提供微调框设定值。
5. 某个字段需要提供进度条显示字段值。
6. 某个字段列需要禁用。
7. 各种委托控件可以设置初始的数据集合，比如下拉框。
8. 各种委托控件在值发生变化的时候发出valuechanged信号，比如下拉框选择声音文件的时候进行播放试听，微调框值改变的时候联动其他控件进行处理等。
9. 某个字段根据设定的规则进行数据校验自动产生不同的图标显示，比如报警红色图标/正常绿色图标，一目了然。同时可设置校验列/校验规则/校验值/校验成功图标/校验失败图标/图标大小。
10. 某个字段根据设定的规则进行数据校验自动绘制不同的背景颜色醒目显示，可设定规则包括 == > >= < <= != contains，可设置符合要求的内容文字颜色/背景颜色。
11. 某个字段需要根据内容显示复选框（自动居中），比如内容是 0/禁用/false 等复选框不选中，1/启用/true 等复选框选中，具体选中不选中对应的内容可自定义。
12. 某个字段需要根据内容重新替换显示成自定义的内容，比如值是0而需要显示成“不符合”字样，1显示成“符合”字样。对应的内容替换规则可设置关键字对照表。
13. 某个字段需要根据颜色值显示对应的颜色，同时可以单击选中进行颜色选择。
14. 某列需要显示操作按钮，按钮的个数/文字集合可设定，根据设定的文字集合平分宽度绘制按钮，单击某个按钮发送对应的按钮单击信号，带按钮索引以及行列，用于用户自行处理。
15. 一个类通用所有需要委托的场景，相当于一个轮子用在所有项目中，不需要单独再去写不同的委托类。
16. 一个类通用所有支持委托的控件，比如QTableView/QTableWidget/QListView/QTreeWidget/QListWidget等。

### 17.3 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_dbdelegate/dbdelegate.gif)

## 18 人脸识别综合应用(在线+离线+嵌入式)
### 18.1 功能特点
1. 支持的功能包括人脸识别、人脸比对、人脸搜索、活体检测等。
2. 在线版还支持身份证、驾驶证、行驶证、银行卡等识别。
3. 在线版的协议支持百度、旷视，离线版的支持百度，可定制。
4. 除了支持X86架构，还支持嵌入式linux比如contex-A9、树莓派等。
5. 每个功能的执行除了返回结果还返回执行用时时间。
6. 多线程处理，通过type控制当前处理类型。
7. 支持单张图片检索相似度最高的图片。
8. 支持指定目录图片用来生成人脸特征值文件。
9. 可设置等待处理图片队列中的数量。
10. 每次执行都有成功或者失败的信号返回。
11. 人脸搜索的返回结果包含了原图+最大相似度图+相似度等。
12. 人脸比对同时支持两张图片和两个特征值比对。
13. 相关功能自定义一套协议用于客户端和服务端，可以通过TCP通信进行交互。
14. 自定义人脸识别协议非常适用于中心一台服务器，现场若干设备请求的场景。
15. 每个模块全部是独立的一个类，代码整洁、注释完善。

### 18.2 人脸识别协议
1. 离线使用，同时支持百度的离线包和嵌入式linux人脸识别静态库。
2. 支持多个连接并发，自动排队处理，返回的时候带上唯一标识区分。
3. 传入单张图片返回人脸区域。
4. 传入单张图片返回人脸特征值。
5. 传入单张图片或者多张图片返回是否是活体。
6. 传入两张图片返回比对结果。
7. 传入两个特征值返回比对结果。
8. 传入单张图片添加人脸。
9. 指定唯一标识符删除人脸。
10. 传入单张照片返回相似度最大的人脸信息。
11. 修改人脸服务的配置参数比如是否快速查找、人脸占比等。

### 18.3 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_video_face/video_face1.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_video_face/video_face2.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_video_face/video_face5.gif)

## 19 硬件综合应用(热敏打印+身份证+短信猫)
### 19.1 串口热敏打印
1. 标准热敏打印协议解析，无依赖，支持任意系统。
2. 可打印各种文字信息比如访客单、报警信息等。
3. 可打印条形码即一维码。
4. 可打印二维码，设置二维码尺寸。
5. 支持多线程打印图片。
6. 可设置打印机的工作模式 0-标准模式 1-翻页模式。
7. 可设置各种边距比如行间距、字符间距、左边距等。
8. 可设置字体信息、字符集、文字对齐、加粗等。
9. 可设置串口号和波特率，不同厂家波特率可能不一致。

### 19.2 身份证阅读器
1. 标准身份证阅读协议解析，无依赖，支持任意系统。
2. 可读取身份证文字信息，比如姓名、性别、名族等。
3. 可读取身份证头像，不同厂家库不一样。
4. 文字信息返回一个信号，头像一个信号，完美。
5. 支持嵌入式linux系统，包括32位64位。
6. 整体流程就是寻找身份证、选取身份证、读身份证信息。

### 19.3 短信猫调试器
1. 标准AT命令协议解析，无依赖，支持任意系统。
2. 可设置收发短信模式 0-text模式 1-pdu模式。
3. 可批量发送短信以及支持长短信发送。
4. 可指定序号读取短信和删除短信。
5. 可一次性删除所有短信。
6. 可检测设备是否运行正常。
7. 支持中文短信发送。
8. 支持拨打电话+挂断电话+接听来电。
9. 可识别用户按键反馈，比如电话另一端按下了什么按键。
10. 支持批量发送给多个号码。

### 19.4 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_hard/hard.gif)

## 20 多线程文件传输工具
### 20.1 功能特点
1. 多线程收发文件，支持加密传输。
2. 接收端支持监听端口接收文件和主动连接服务器接收文件两种方式。
3. 按照 文件开始符+文件大小+文件内容+文件结束符 逐个分包接收。
4. 可对接收的加密过的文件包进行解密输出。
5. 如果采用连接服务器方式接收文件可指定请求文件。
6. 接收端请求文件的形式可以作为通用的程序升级方案。
7. 进度条实时更新收发文件的进度。
8. 发送端可设置每个包最大大小即切片分包数量。
9. 发送端可对文件的每个包进行加密传输。
10. 发送端支持对包进行合并发送。
11. 可指定目录对客户端发来的请求文件进行搜索。
12. 每个功能独立的一个类，接口清晰友好，使用方便。
13. 支持任意Qt版本、任意系统、任意编译器。

### 20.2 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_tcpfile/tcpfile.gif)

## 21 雨田哥作品专区
### 21.1 雷达模拟仿真工具
1. 支持音频频谱显示。
2. 支持任意随机添加模拟点。
3. 支持自定义添加模拟点。
4. 支持方位、航向角、距离、速度、目标体真实图自定制。
5. 支持危险区域范围显示。
6. 支持激光发射模拟。
7. 支持雷达图放大缩小显示。
8. 支持模拟点编辑设置。
9. 支持模拟点跟踪线设置。
10. 支持模拟点详细数据查看。
11. 支持自定义换肤。

2.0版本
1. 增加添加目标体预览功能。
2. 增加航母目标体。
3. 增加歼击机目标体。
4. 增加指挥所目标体。
5. 增加航母炮弹攻击指挥使效果。
6. 增加航母导弹攻击指挥使效果。
7. 增加歼击机炮弹攻击指挥使效果。
8. 增加歼击机导弹攻击指挥使效果。
9. 增加指挥使被炸前、中、后三种状态效果。

### 21.2 录音播放控件
1. 使用FMOD音频引擎开发，支持跨平台、虚拟频道、插件设计。
2. 数字回放、多个声卡、多路输出、多路输入。
3. 自定义回放延迟、网络特性。
4. 支持类型：DLS、M3U、ASX、WAX、PLS、AIFF、ASF、FLAC、FSB、MOD、MP2、MP3、OGG、RAW、S3M、WAV、WMA、XM、VAG。可以说是相当的牛逼。
5. 录音(自动保存WAV文件) 实时播放。
6. 支持声道、采样频率等设置。
7. 播放音频文件。
8. 音频频谱图显示。
9. 音频瀑布频谱图显示。
10. 背景色、频谱色可调。
11. 录音时长、音频文件播放时长显示。
12. 支持开始录音、暂停录音、停止录音操作。

### 21.3 PDF阅读器
1. 仿WPS界面。
2. 预览PDF文件。
3. 支持PDF预览放大、缩小。
4. 支持目录预览查看。
5. 支持目录点击跳转页查看。
6. 支持页数指定跳转。
7. 支持上一页、下一页、首页、尾页跳转。
8. 支持鼠标拖拽滑动预览。
9. 支持换肤。
10. 动画Tab页。
11. 支持实际大小、适合页面、适合宽度、预览跳整。
12. 支持工具栏、类目栏拖拽位置调整、隐藏。
13. 可定制各种功能。

2.0版本
1. 支持Mac、Linux、Windows平台环境。
2. 增加实际大小、页面、窗口宽度比例调节设置。
3. 增加窗口拖拽和拉伸。
4. 增加PDF预览修改功能。
5. 选择工具-选中文本进行剪贴板的复制和粘贴操作。
6. 增加文本选中、高亮、下划线、删除线编辑操作。

### 21.4 效果图
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_yutian/radar1.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_yutian/radar6.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_yutian/audiorecord.gif)
![avatar](https://github.com/feiyangqingyun/QWidgetExe/raw/master/snap_yutian/pdfreader1.gif)