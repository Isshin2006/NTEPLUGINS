# NTE 改装工具箱（两个 Anomaly 插件）

两个 Anomaly 3.0 插件，AGPL-3.0 开源，源码全部在本仓库内。

## 一、载具改装召唤+实时改装（NteVehicle 改造版 v0.11.35）

基于官方 NteVehicle v0.11.1 改造。功能：每车改装记忆与改装召唤、**实时改装当前乘坐载具**（全部改装类别+涂装+特效白名单，行驶中即时生效）、双模式传动调校（最高限速/升降档转速/换挡耗时/齿比等，拖动即生效）、每车调校记忆、诊断工具、日志导出。

## 二、AutoTaxi 自动出租车（b1ank 原版改造 v0.2.0）

基于 b1ank 的 AutoTaxi 0.1.11 改造。功能：自动接客/送达/结算循环；**多角色自动队列**——勾选多个想要的偶遇角色，队列按顺序逐单自动预选，今日不可遇自动跳过保留；勾选持久化（重启不丢）。

## 安装（手动，一分钟）

1. 打开本仓库右侧 **Releases** → 下载对应的 zip：
   - `NteVehicle-0.11.35.zip`（载具改装+实时改装）
   - `Autotaxi-0.2.0.zip`（自动出租车+多角色队列）
2. 解压后把里面的 `NteVehicle\` 或 `Autotaxi\` 整个文件夹放进游戏目录的
   `Anomaly\plugins\` 下（同名文件夹直接覆盖）；
3. 重启 launcher 和游戏，在插件管理器里启用。

## 构建源码

- NteVehicle：`NteVehicle/src/build_27.bat`（需官方 Anomaly 2.7 源码树，见脚本内说明）
- AutoTaxi：官方仓库 `Anomaly-main` 树下 MSVC 直编（参考 b1ank 原版构建方式）

所有改动均带 `Local fix/Local feature` 注释标记，欢迎接手与改进。

## 许可

两个插件均为 **AGPL-3.0-only**（继承自官方 Anomaly 与 b1ank 的 AutoTaxi）。
致谢：AnomalyNTE 官方团队、b1ank（AutoTaxi 原作者）。
本插件仅修改本机客户端数据，不影响他人；使用产生的风险自行承担。
