# HPMAMagicQuiz CPU 版（下载即用）

《哈利波特：魔法觉醒》魔法史答题助手 —— 免安装 exe。

## 下载

到 [Releases](https://github.com/dejectedraven/HPMAMagicQuiz-Release/releases) 页面下载最新版
`HPMAMagicQuiz-CPU-v1.2.2.exe`（单文件约 115 MB）。

## 使用

1. 双击 exe（会弹 UAC，选"是"）
2. 输入授权号（找管理员要）
3. 游戏保持 2560x1440 全屏，按 **F8 开始** / **F9 停止**
4. 首次运行会在 exe 旁边生成：
   - `data/questions.csv` 题库（自动学习会写入这里）
   - `logs/` 运行日志
   - `config.json`（需要改配置时自己新建）

## 常见问题

- **鼠标不动/点击无效**：必须管理员运行（exe 已内置管理员清单，双击弹 UAC 即可）
- **想用 GPU 加速**：本版是 CPU 版（单题约 1 秒）；GPU 版需要单独装 CUDA 环境
- **更新程序**：下载新版 exe 覆盖旧的即可，题库和配置在旁边不会被覆盖
- **报毒**：PyInstaller 打包的 exe 偶尔会被杀软误报，加白名单即可

## 数据自动同步（不用重新下载 exe）

启动时会从发布仓库自动拉取：

- **白名单**（`whitelist.json`）：管理员加/删授权号后，用户下次启动自动生效
- **题库**（`bank.json` + `data/questions.csv`）：管理员更新题库后自动合并
  （同题以管理员版本为准，用户自己学到的独有题目保留）
- 拉不到网络时用本地缓存/内置版本，**离线照样能用**

## 版本

当前版本：v1.2.2（见 `latest.json`）

仅供学习交流，请自行评估风险（包括游戏账号风险）。
