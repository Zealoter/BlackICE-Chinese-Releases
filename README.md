# 黑冰中文版 v1.2.1 完整安装版

这是面向《钢铁雄心 3：他们最美好的时刻》4.02 的非官方黑冰中文汉化与界面改进版。本包包含完整的黑冰中文版 MOD 资源、字体、界面及本机兼容补丁。请支持正版 HOI3 及资料片。

## 从正版游戏直接安装

1. 安装正版 Windows 版 HOI3 TFH 4.02。退出游戏，把完整安装包解压到有足够空间的独立目录。本包可直接安装在正版游戏上。
2. 在解压目录打开 PowerShell，运行以下命令。将 `-GameExe` 的路径换成你的游戏路径。

   ```powershell
   New-Item -ItemType Directory -Path ./patched
   & ./tools/Apply-Compatibility.ps1 -GameExe 'D:/Games/Hearts of Iron 3/hoi3_tfh.exe' -OutputDirectory ./patched
   ```

3. 看到 `Verified output` 后，备份游戏目录里的 `hoi3_tfh.exe` 和现有同名 MOD。把 `patched/hoi3_tfh.exe` 和包内 `hoi3` 下的 `tfh` 文件夹复制到游戏根目录，选择 `BlackICE GitHub Chinese` 启动。

补丁支持通过哈希验证的 Steam TFH 4.02 原版、黑冰中文版 v1.0.1 及当前兼容版本。其他可执行文件会提示不受支持。安装前可用发布页附带的 SHA-256 校验值验证 ZIP。老玩家可先备份存档和已有 MOD，再更新。

## 本版内容

- 国旗下的国家加成支持滚动查看，科技详情悬停即显示每级与累计效果，并按内容调整高度。
- 恢复地图红绿战斗气泡数字，用户已在游戏中确认。
- 补齐地图及旋转文字中的缺字，调整建筑悬停提示的中英文字距，整理两层的将领特性进度文本。其余界面细节继续接受游戏内反馈。

下一轮关注生产 IC 不足的红字、战斗详情排版、军指挥部文字遮挡和将领头像缺失。小国科研补偿和技术交易属于独立玩法议题。

本项目是免费的玩家 MOD，游戏本体需自行通过正版渠道安装。Black ICE、既有汉化和其他第三方素材权利归各自作者，出处见 `CREDITS.md`。
