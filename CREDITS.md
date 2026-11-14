# 鸣谢与出处

本项目是**整合**，不是从零做的。绝大部分内容来自别人，这里把出处写清楚。

## 游戏

**《钢铁雄心 3：他们的最美好时刻》(Hearts of Iron III: Their Finest Hour) 4.02**
© Paradox Interactive。本项目**不包含游戏本体**，任何游戏原始资源的使用都应以你拥有
该游戏的正版授权为前提。

## MOD 本体

**Black ICE**（HOI3 的大型 AAR/历史向 MOD）
- 仓库：<https://github.com/oumajgad/BlackICE>
- 本项目包含其 MOD 内容（`common`、`events`、`decisions`、`history`、`gfx`、`map`、
  `units`、`technologies`、`localisation`、`music`、`sound` 等），并按原样随包分发。
- 版权归 Black ICE 制作组及各自作者。音乐与美术资源版权归各自权利人。
- 如果权利方不希望这些内容出现在本仓库，联系我，我会移除对应部分。

## 中文文本与字体

**《钢铁雄心3 TFH 402 汉化第三版》**
- 提供了汉化的**字形图集**（`Arial14chi` / `Arial16chi` / `Arial30chi` / `Arial45chi` 等
  GB2312 位图字体）和**基础中文文本**，是本项目能显示中文的前提。
- 版权归原汉化组。

**ParaTranz「HOI3 Black ICE CN」项目**
- 项目页：<https://paratranz.cn/projects/18898>
- 本项目通过脚本（`tools/merge-paratranz.py`）把该项目导出的**人工译文**合并进来，
  人工译文优先于其他来源。
- 版权归该项目及所有贡献者（遵循 ParaTranz 该项目声明的许可）。

## 本项目自己做的

- **整合**：Black ICE 与汉化文本逐 key 合并（汉化有的 key 用中文，BI 独有的 key 保留英文），
  汉化字体声明与 BI 的 `interface/core.gfx` 合并，保留 BI 独有的字体名。
- **引擎补丁**：8 位→16 位字形补丁的现场分析与落地（42 处补丁点 + 新增代码段）、
  `0xC0000005` 崩溃的根因定位与 2 字节修复、LAA 标志。
- **界面修复**：顶栏 5 个数字框改用半角位图字体（去掉数字前 12px 空白、避免 6 位数换行）、
  IC 框宽 95→100px。
- **文本**：105,000+ 条名目（将领 / 部队番号 / 内阁部长）的中文化，
  以及本地化文本从 60.1% 补到 95.8% 的部分。
- **工具**（`tools/`）：翻译流水线、覆盖率统计、字体图集离线预览、界面自检、
  分辨率设置、冒烟测试。

## 引用

如果你要再分发或在别处引用本项目，建议照抄下面这段：

```
黑冰中文版 (Black ICE Chinese for HOI3)
= Black ICE (https://github.com/oumajgad/BlackICE)
+ 钢铁雄心3 TFH 402 汉化第三版
+ ParaTranz HOI3 Black ICE CN (https://paratranz.cn/projects/18898)
+ 整合、引擎补丁、界面修复与剩余翻译（本项目）
```
