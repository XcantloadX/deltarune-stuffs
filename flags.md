flag 从存档文件的第 317 行开始

例如：  
flag[0] 为 存档文件中的第 317 行  
flag[16] 为 存档文件中的第 317 + 16 = 333 行   
flag[209] 为 存档文件中的第 317 + 209 = 526 行  

（注：0 为 false，1 为 true）  

---

|  行号   | 数据类型 |    范围     |                             说明                             |  状态  |
| :-----: | :------: | :---------: | :----------------------------------------------------------: | :----: |
|   0-5   |   bool   |             |                            未使用                            |        |
|    6    |   bool   |             |                             未知                             |        |
|    7    |   bool   |             |                             未知                             |        |
|    8    |   bool   |             |    可能为设置里的“简化视觉效果”，影响到 Jevil 的战斗背景     | 待验证 |
|    9    |   bool   |             |                    可能与 battle 音乐有关                    |        |
|   10    |   bool   |             |         是否与 room_drak1 房间里的闪烁的星星进行对话         |        |
|   11    |   bool   |             |                       是否启用自动奔跑                       |        |
|   12    |   bool   |             |                      设置里的 shakeoff                       | 待验证 |
|   13    |   bool   |             |                             未知                             |        |
|   14    |  bool?   |             |                             未知                             |        |
|   15    |  float   | 0<=float<=1 |                            总音量                            |        |
|   16    |  float   | 0<=float<=1 |                         背景音乐音量                         |        |
|   17    |  float   | 0<=float<=1 |                           音效音量                           |        |
|  18-19  |          |             |                            未使用                            |        |
|   20    |   int    |             |              未知（在许多毫不相干的脚本里都有）              |        |
|  21-28  |          |             |                            未使用                            |        |
|   29    |  bool?   |             |                             未知                             |        |
|   30    |   int    |  0<=int<=2  | Raisel 对话框贴图选择（0:默认,   1:戴帽子（类似UT里的船夫）, 2:取下帽子（暗世界结尾时）） |        |
|   31    |   bool   |             |                        是否启用脚步声                        |        |
|   32    |   bool   |             |                 可能与彩蛋房间 room_man 有关                 | 待验证 |
|   33    |   int    |             |        计时器，用来计时（目前只用在与 sans 的对话上）        |        |
|  34-39  |          |             |                            未使用                            |        |
|  40-60  |          |             |                           暂时跳过                           |        |
|   53    |  bool?   |             |                          可能未使用                          | 待验证 |
|  54-99  |          |             |                            未使用                            |        |
|   100   |   bool   |             |            room_dark3a 中的闪光的碎片是否去取出来            |        |
| 101-103 |   int    |  0<=int<=2  |         某房间里可以拿 2 个黑暗糖果的树上剩下的糖果          |        |
|   104   |          |             |                            未使用                            |        |
|   105   |   bool   |             |                  监狱里的铁制镣铐是否被拿走                  |        |
|   106   |   bool   |             |                    监狱里的苔藓是否被吃掉                    |        |
|   107   |          |             |                            未使用                            |        |
|   108   |   bool   |             |       未知（影响一个对话，此 flag 与 flag[233] 联动）        |        |
| 109-111 |          |             |                            未使用                            |        |
|   112   |   bool   |             |   为 true 时，room_cc_prison_prejoker   房间中的箱子会消失   |        |
| 113-114 |          |             |                            未使用                            |        |
|   115   |  bool?   |             | 大于等于 1   时，第一个商店里的谈话选项里的“奇怪的犯人”会变为白色 |        |
| 116-199 |          |             |                            未使用                            |        |
|   200   |  bool?   |             | 触发“*   嘿，你走的还挺快。”（Susie 对话）时会被设置为 true ，可能未使用 | 待验证 |
|   201   |   bool   |             |         未知（与开头的黑暗之眼（darkeyes）谜题有关）         | 待验证 |
|   202   |   int    |             | 触发“*   老天哪。得了吧。 * 你连路都不知道呢。”（Susie 对话）时会被设置为 2，触发“* 呼...噗…  * 什么，你想赛跑吗？”时会被设置为 1，可能未使用 |        |
|   203   |  bool?   |             |                       未知（影响对话）                       | 待验证 |
|   204   |   int    |             |                       未知（影响对话）                       | 待验证 |
|   205   |   int    |             | 在教程里：人偶满血且 Miss 次数等于 9 时设置为   6，攻击人偶次数大于 3 时设置为 4，此值大于等于 4 时会触发“* 抱歉，Kris。?  * 下次我会试着做个更好的老师。”（Raisel   对话）以及“*（哦，Kris！*     Susie也没学过教程！）” |        |
|   206   |  bool?   |             |                           影响对话                           |        |
|   207   |   int    |             |         0-没有把手册扔在地上，1-扔过一次，2-扔过两次         |        |
|   208   |   bool   |             |                在战斗中说服方钻后设置为 true                 | 待验证 |
|   209   |   bool   |             | 是否已显示 Field of Hopes and Dreams   Logo（在第一次进入平原时会显示） |        |
|   210   |   int    |             | 影响 room_field2 房间里的 obj_event   和obj_npc_facing 对话  |        |
|   211   |   int    |             |                             未知                             |        |
|   212   |   int    |             |        未知，影响 room_field_boxpuzzle   房间里的谜题        |        |
|   213   |          |             |                            未使用                            |        |
|   214   |   int    |             | 队伍名字（1-“$！？#小分队”，2-“Lancer 粉丝俱乐部”，3-“快乐帮”） |        |
|   215   |  bool?   |             | 未知，此 flag 与 flag[251] 联动，此 flag   为 1 则flag[251] 也为 1，当此 flag 为 0 时obj_npc_puzzlemaster1 会被销毁 | 待验证 |
|   216   |   bool   |             |                     是否给平原的教程捐款                     |        |
|   217   |   bool   |             |             是否已完成 Rouxls Kaard 的第一个谜题             |        |
|   218   |   bool   |             |             是否已完成 Rouxls Kaard 的第二个谜题             |        |
|   219   |          |             |                            未使用                            |        |
| 220-226 |          |             |                  未知，与 Lancer 的机器有关                  | 待验证 |
| 227-228 |          |             |                            未使用                            |        |
|   229   |          |             |                  未知，与 Lancer 的机器有关                  | 待验证 |
|   230   |          |             |                            未使用                            |        |
|   231   |          |             |              未知，与 Susie 在监狱里的解谜有关               | 待验证 |
|   232   |   bool   |             |         是否与 room_forest_area1 房间的“蜜蜂罐”对话          |        |
|   233   |   bool   |             |                             未知                             | 待验证 |