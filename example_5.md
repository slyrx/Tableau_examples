### 通过 一份 模拟 的数 据进 行欺诈 检 测 
在保险 业 , 数 据分析技术 主要用于新客户 的获 取分析、产 品的购 物篮 分析、客户 细 分、客户 流失 以及欺诈 检 测 分析，等等。

#### 方法

步骤：
1. 打开 软 件并 读 入“欺诈 检 测 .Xls”数 据。
2. 建两 个 新的字段，"赔 付金额 比例”和 “总 事故数 ’
3. 右击 度量中的字段"总 支付额 ”，
4. 择 【创 建计 算字段】
5. 命名为 "赔 付金额 比 例 ’ ’
6. " 赔 付 金 额 比 例 ” = S U M ( 总 支 付 额 )/ S U M ( 总 索 赔 额 
7. 右 击 度 量 中 的 字 段 " 保 险 单 号 "
8.  选 择 【 创 建 计 算 字 段 】
9. 命 名 为 ‘ ‘总 事 故 数 "
10. “总 事 故 数 = C O U N T ( 保 险 单 号 )
11. 再创 建一个 可结 合实 际 调 整的参 数 
12.  其命名为 "可控指数 "
13.  择 【创 建参 数 】，
14. 数 据类 型定义 为 "浮点"，最小最大值 分别 定义 为 0.5 和0.9,
15.  创 建一个 字段
16. 来 判断 "赔 付金额 比例" 是否大于我们 定义 的"可控指数 
17. 命 名 为 " 阀 值 判 别 
18. 新建一张 工作表
19. 将 "总索赔额”和"总事故数"分别放入【列】和【行1
20.  记 图 形 选 为 【 形 状 】， 
21. 并 在 形 状 中 选 择 一 个 " 人 形 ” 的 图 标 
22. 将 "阀值判别”、"总支付额”分别放入【颜色】框和【大小】框
23. 再把市级 ”放入【详 细 信息】中，
24. 并 在视 图 区 中右击 ，选 择 【趋 势 线 ]〇
25. 在 视 图 区 中 右 击 ， 选 择 【趋 势 线 】一 I 编 辑 趋 势 线 1 , 将 " 显 示 置 信 区 间 前 边的钩 去掉。
26. 单 击 菜 单 栏 【 格 式 】 一 【 阴 影 】， 为 视 图 选 择 一 种 背 景 颜 色
27. 分别 显 示"总 索赔 额 "、"总 支付额 "、"区 域"和 "可控指数 ”的怏速筛选 器
28. 最后将 此视 图 置入一张 新建的仪 表板中

### 模拟 了两 台机器的生产 运 营 数 据，对 其相关 问 题 进 行分析
制造业 有着非常复 杂 繁多的数 据，数 据可视 化在制造业 中有着极 其重要的作用， 提升设 备 利用率、优 化资 源组 合对 提升企业 运 营 效率、增加企业 收益有着重要意义 。

1. 打开 软 件并 读 入"工艺 生产 分析.xls-订 单 数 据.sheet"
2. 将 "机 型”、"订 单 号 ”从 【度量】拖到丨 维 度]〇
3.  据 已 有 字 段 构 造 两 个 新 的 字 段 ， 分 别 是 " 实 际 停 机 时 间 ” 和 " 实 际 产 量 ”。
4. 右击 度量中的字段"记 录 停机时 间 ”，
5. 选 择 【创 建计 算字段】，
6. 构 造字段"实际停机时间"，其中"实际停机时间”="记 录 停机时 间 "未记录停机时间 "
7. 右击 度量中的字段"过 生产 量’，
8. 选 择 【创 建计 算宇段】，
9. 创 建字段"实 际产 量 ”， 其 中 " 实 际 产 量 ” " 过 生 产 量 常 规 生 产 量 ”
10. 分别 把字段"差异 (元)"和"计 划 产 量”放入【行】和【列】中，
11. "机型”放 入 【颜 色 】框 中 。
12. 标 记 图 形选 为 【圆 ]，并 设 置圆 形“边 界_’，来 美化视 图 
13. 再把“订 单 号 ”、'‘开 始时 间 ”、“预 计 停机时 间 实 际 停机时 间 "、“实 际 产 量"、“实际设置时间(时 )"、“预期设置时间(时 实 际 运 行时 间 (时 )”和“预 计运行时间(时 )"放入【详细信息】框中
14. 将 "开始时间”格式设置 为 "年/月/日_’，
15.  预 计 值 和实 际 值 并 列对 比显 示
16.  击 菜单 中【工作表】选 择 【工具提不丨 
17.  整框 中字段的顺 序等对 工具提示进 行个 性化设 置
18.  建一个 参 数 ，我们 将 其命名为 “度量"。
19. 右击 "度量”列表框 中的空白处 ， 选 择 "创 建参 数 ”，
20.  造 4个 新的字段，分 别 是 "度量单 位"、"度量指数 "、"期望度量值 ”和 “实 际 度量值 ”
21. 右击 参 数 中的"度量”，选 择 【创 建计 算字段】，构 造字段“度量单 位”
22. 右击 参 数 中的"度量’，选 择 【创 建计 算字段】，构 造字段"期望度量值 ",
23. 右击 参 数 中的"度量"，选 择 【创 建计 算字段】，构 造字段"实 际 度量值 ",
24. 右击 参 数 中的"度量"，选 择 【创 建计 算字段】，构 造字段"度量指数 "
25. 在 【 标 记 丨 处 将 图 形 类 别 选 为 “条 形 图 " ， 
26. 把 " 期 望 度 量 值 " 和 ‘ ‘开 始 时 间 H 分别放到【列】和【行】上，将 "期望度量值"的聚合改为平均值，并右击行 上的"开 始时 间 ”将 其设 置为 连 续 类 型【曰】，并 将 其转 换 为 【离 散1〇
27. 把 " 实 际 度 量 值 “度 量 单 位 " 、 ‘ ‘度 量 指 数 " 和 “度 量 ” 均 放 入 【详 细 信 息 I 框 中
28.  条 形图 变 成子弹 图 ，完成预 计 值 与 实 际 值 的差异 分析
29. 右击 "期望度量值"的坐标轴下方，
30. 选 择 【添加参考线】，弹出编辑窗口
31. 将 添加第一种 和第三种 ，分别 用【标 签 】和 【颜 色I将 实 际 值 和预 计 值 进 行清 晰 的对 比
32.  接数 据“工艺 生产 分析.xls-机器状 态 记 录 sheet"，
33. 在数 据窗 口中，将 "订 单 号 ”从 【度量】拖到【维 度】。
34. 新建一张 工作表，对 机器的状 态 进 行分析。
35. 定 义 两 个 新 的 字 段 ， 分 别 是 " 持 续 时 间 ( 分 )” 和 " 持 续 时 间 ( 天 )” ， 
36. 在 标 记 处 选 择 " 甘 特 条 形 图 " ， 
37. 把 “开 始 时 间 ” 拖 放 至 【 列 】 上 ， 并 将 其 格 式设 置为 "精确 日期”，把 “状 态 "拖放至【行】上。
38. 再将 "状 态 ”放入【颜 色】框 中。
39.  持 续 时 间 ( 天 )” 放 入 【 大 小 】 框 中 。
40. " 订 单 号 " 、 " 结 束 时 间 ” 和 “持 续 时 间 ( 分 ) " 放 入 【 详 细 信 息 】 框 中 。
41. 新建一张 仪 表板，
42. 将 前面 做好的三个 工作表添加到仪 表板中
43. 单 击 "订 单 分析"视 图 右上角的下拉菜单 按钮 ，
44. 选 择 菜单 选 项 中的"用作筛 选 器"，
45. 把 "订 单 分析"视 图 设 置为 筛 选 器。
46. 添加一种 背景颜 色

### 模拟 的一份 能源行业 的数 据
1. 读 入 数 据 "资 源组 合分析.xls"
2. 在数 据窗 口中，将 "地名”从 【度 量 】 拖到【维 度1〇
3.  "累积石油量(立方米)"和‘'累积水量I立方米r分别放入丨行】和【列】 中。
4. 【标 记 】下拉菜单 中选 择 图 形为 [形状 ]
5. 为了更加美观，形状选为I 。
6.  "地名"和 “年份 _’放入【详 细 信息】框 中
7. 设 置均值 线 、趋 势 线 等。
8. 首先设 置均值 线 
9. 右击 横 轴 坐标 轴 下方区 域，选 择 【添加参 考线 】，
10. 右击 纵 轴 坐标 轴 左方区 域，选 择 【添加参 考线 】
11. 接着，在视 图 中添加一条 趋 势 曲线 。
12. 在视 图 区 单 击 右键 ，选 择 【趋 势 线 】
13. 右 键选择【趋势线】— 【编辑趋势线】，将 "显示置信区间”前边的勾去掉
14. 添加一种 背景颜 色
15. 选 中这 条 趋 势 线 再右击 
16.  择 【编 辑 趋 势 线 】
17. 尝 试 用不同类 型的曲线 进 行拟 合，例如选 择 三次曲线 
18. 添加其他辅 助分析的参 考线 ，如置信曲线 、四分位线 等
19. 右击 横 轴 坐标 轴 下方区 域，选 择 【添加参 考线 】，
20. 右 击 纵 轴 坐 标 轴 区 域 ， 选 择 【 添 加 参 考 线 】
21. ，添加快速筛选器，右击 1‘年份”、“断块类型"和"水率(升/天)”，选 择 [显 示快速筛 选 器1〇
22. 制作播放器
23. 再次将 ‘年份 ”从 左侧 维 度列表中拖人I页 面丨 框 中，单 击 hiara 键 ，可按照"年份 '’逐年播放
24. 最后，新建一张 仪 表板，将 刚 做好的工作表添加到仪 表根中
