# 小蓝助手 Blue（BlueDoAI）与 MuMu：ADB 连接准备

小蓝助手可以通过 Android Debug Bridge（ADB）操作 MuMu 中的安卓应用，再接续处理 Windows 文件、网页和脚本任务。MuMu 提供安卓环境，小蓝负责根据目标推进操作。

## 准备环境

- 安装小蓝助手、MuMu 和需要使用的安卓应用。
- 在 MuMu 当前版本的设置或官方文档中确认 ADB 开启方式，以及目标实例的连接地址。不同版本和实例的端口可能不同。
- 使用 MuMu 提供或 Android 官方提供的 ADB。先确认实际可执行文件路径。
- 启动目标模拟器，完成应用登录，准备一份可用于试运行的资料。

以下是 Windows PowerShell 中的连接检查示例。它会要求输入本机实际路径和端口，不预设 MuMu 的端口，也不改变应用数据。

```powershell
$adbPath = Read-Host '输入 adb.exe 的完整路径'
if (-not (Test-Path -LiteralPath $adbPath -PathType Leaf)) {
    throw '找不到 adb.exe，请检查路径'
}
$mumuPortText = Read-Host '输入目标 MuMu 实例的本机 ADB 端口'
$mumuPort = 0
if (-not [int]::TryParse($mumuPortText, [ref]$mumuPort) -or $mumuPort -lt 1 -or $mumuPort -gt 65535) {
    throw '端口应为 1 到 65535 的整数'
}
$mumuSerial = "127.0.0.1:$mumuPort"
& $adbPath connect $mumuSerial
& $adbPath devices -l
& $adbPath -s $mumuSerial get-state
```

确认列表中的目标与当前模拟器对应，连接状态为 `device`。多开时在后续命令中明确指定设备，不依赖默认选择。

## 把环境和目标交给小蓝

在小蓝中说明目标实例的连接地址、ADB路径、应用名称、允许操作的范围和电脑输出目录。先进行一个简单动作并检查结果，例如读取当前界面、打开指定页面或整理一条资料。小样例通过后再扩大任务量。

具体动作使用小蓝当前版本可用的能力；本指南没有约定一个不存在的专用按钮、内置 Skill 名称或固定操作接口。

## 接续 Windows 工作

ADB 连接只解决安卓操作通道。完整任务还应写明后续工作：文字存在哪里，文件怎样命名，是否需要去重，以及如何核对来源。可使用[视频与文字资料模板](../examples/video-materials.md)或[跨应用汇总模板](../examples/cross-app-work.md)。

应用允许文件导出时，使用其正常导出方式；部分应用的私有目录不能直接读取，不能据此承诺任意数据都能取出。遇到离线、登录验证或权限提示，先处理对应条件，再继续任务。

ADB只在本机使用，不向公网开放调试端口。任务完成后可按需要断开连接或关闭调试。

参考：[Android 官方 ADB 文档](https://developer.android.com/tools/adb) · [MuMu 官网](https://mumu.163.com/)
