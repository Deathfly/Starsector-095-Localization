﻿﻿﻿# Starsector-095-Localization

## Python环境: 3.8.5
| 文件                                  | 作用                                                        |
| ------------------------------------- | ----------------------------------------------------------- |
| handleVariantNames.py                 | 处理指定文件夹中所有装配名，并更新/使用映射 json 用于翻译。 |
| swapLangFile.py                       | 用来更替汉化文件和英文文件的脚本。                          |
| FindDifference.py                     | 查找不同版本之间的差异。                                    |
| variant_name_map.json                 | 装配名映射文件，英文名对应汉化名，可后继继续更新。          |

## 文件夹内容

* "版本号 + data"是游戏版本 data 文件夹
* "localization" 指的是需要翻译的内容
* "original" 指的是相应的英文原版内容，不要改动(如果有漏的就加进 original 和 localization)

## 注意
目前大内容只剩下 rules.csv 和校对，请希望帮助汉化的小伙伴们先联系汉化组。

通过 QQ 553816216 添加 **议长** 的好友，注明你的来历和英语水平，务必在申请时说清，不然只能请通过QQ群私聊联系。

添加需要翻译的内容时，先复制到 **original** 文件夹备份，然后再复制到 **localization** 文件夹进行翻译。

## 标点符号规范

* 关于文本内的中英文符号使用规范：
  * 仅应当使用中文逗号`，`与中文句号`。`。中文问号`？`、感叹号`！`与括号`（）`因其不美观而不应当使用。
  * 相应地，在能使用中文逗号或中文句号的场合，应当尽可能使用它们而非英文逗号和英文句号。
  * 省略号建议以三个英文逗号`...`表示，六个英文逗号因过长而不美观。
* 使用`{}`来包括部分词语：
  * 人名应当由`{}`包括，且括号的两侧不应该出现额外空格，例如`舰长{Peter}在一次战斗中取得了胜利。`
  * 英文地名也应当类似地使用`{}`包括，且括号的两侧不应该出现额外空格，例如`前往{Galatia}学院接受任务。`
  * 需要强调的英文词组或短句也一样，例如`发送你的{PID}到目标处。`
  * 此外，**所有以`$`为开头的token必须以`{}`包括，以避免潜在的BUG**，例如`这将花费{$cost}星币。`
  * `{}`包括**必须以`}`作为结尾闭合，否则将产生过长字符串捅穿屏幕的问题**。在`{}`闭合的情况下，此类问题目前不再发生。

## 译名表
在这里放置统一译名。

| 英文名                  | 译名               | 注释                       |
| ----------------------- | ------------------ | -------------------------- |
| Comm link               | 通讯链接           | 请注意`链接`和`连接`的区别 |
| Cut comm link           | 切断通讯链接       | 同上                       |
| credit/credits          | 星币               | 请不要翻译成信用           |
| hegemony                | 霸主               | 请不要翻译成霸权主义       |
| Janus Device            | ""双面神""装置     |                            |
| [REDACTED]              | [数据删除]         |                            |
| Nav Buoy                | 导航浮标           |                            |
| Sensor Jammer           | 传感干扰器         |                            |
| Sensor Array            | 传感器阵列         |                            |
| Comm Relay              | 通讯中继站         |                            |
| Probe                   | 探测器             |                            |
| Warning Beacon          | 警告航标           |                            |
| Fusion Lamp             | 聚变射灯           |                            |
| Yellow Star             | 黄矮星             |                            |
| Orange Star             | 橙矮星             |                            |
| Contacts                | 联络人             |                            |
| Galatia Academy         | Galatia 学院       | 在rules等地请适当加上`{}`  |
| Galatia Academy Station | Galatia 学院空间站 |                            |
| mote                    | 光尘               |                            |
| Hypershunt Tap          | 超分流阀门         |                            |
| Coronal Hypershunt      | 星冕分流器         |                            |


## 修正表
在这里放置统一译名。

| 英文名          | 旧译名     | 新译名       | 理由     |
| --------------- | ---------- | ------------ | -------- |
| Enforcer        | 压迫者     | 执法者       | 词不达意 |
| SafetyOverdrive | 安全超载   | 安全协议超驰 | 词不达意 |
| Gryphon         | 鹰头狮     | 狮鹫         | 遗留问题 |
| Graviton Beam   | 引力子激光 | 引力子束     | 词不达意 |
