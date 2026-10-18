# 小蓝助手 Blue（BlueDoAI）

**智能体处理不了的工作，找小蓝助手。**

智能体提示“无法操作这个软件”“没有可用工具”，或找不到办法完成任务？可以把目标和资料交给小蓝助手，尝试在实际应用中完成工作。工业工艺与研发、PS图片处理、复杂脚本、安卓应用操作、视频与文字资料整理，都可以从一项具体任务开始。

小蓝助手 Blue 是自研的 Windows 执行型 AI 智能体。它可以拆解多步骤任务，编写和运行脚本，操作支持的应用与网站，并把文件、脚本和处理记录留在项目目录中，方便检查和修改。结合 MuMu 安卓模拟器，小蓝还可以通过 ADB 操作安卓应用，将电脑端与安卓端的工作接起来。

[下载 Windows 版](https://github.com/ffawei/xiaolan-assistant-bluedoai/releases/latest) · [产品介绍](https://www.bluedoai.com/legal/product-overview/) · [模型与价格](https://www.bluedoai.com/model-plaza) · [企业服务](https://www.bluedoai.com/enterprise/) · [English](README.en.md)

## 下载安装

当前正式版本：**1.11.31（Windows）**。

- [直接下载安装程序](https://github.com/ffawei/xiaolan-assistant-bluedoai/releases/download/v1.11.31/xiaolan-1.11.31-setup.exe)
- [最新发行页](https://github.com/ffawei/xiaolan-assistant-bluedoai/releases/latest) · [所有版本](https://github.com/ffawei/xiaolan-assistant-bluedoai/releases)
- [官网与国内下载渠道](https://www.bluedoai.com/tools/)

普通用户下载 `.exe` 安装程序即可。发行页的 `.blockmap` 和 `latest.yml` 是配套更新文件，`SHA256SUMS.txt` 用于校验下载结果。GitHub自动生成的“Source code”压缩包是本仓库文档，不是小蓝安装包。

GitHub提供已公开发行文件的原样镜像，安装包已与原发行元数据核对。1.11.30作为历史版本保留；现有客户端自动更新地址保持原样。

## 哪些工作可以找小蓝

| 工作 | 可以怎样交代目标 | 要检查的成果 |
| --- | --- | --- |
| 工业工艺与研发复杂任务 | 结合给定的工艺文件、试验记录和研发要求，整理资料、运行数据处理脚本，核对版本与待确认问题 | 来源对应的资料表、分析脚本、计算结果、变更与问题清单 |
| Photoshop（PS）图片处理 | 根据图片、尺寸和参考要求处理素材，保留原文件，另存结果 | 输出图片、尺寸、命名；任务要求时保留可编辑文件 |
| MuMu 安卓应用操作 | 通过 ADB 连接指定模拟器，完成支持的应用操作，并将相关资料整理到电脑 | 文件、来源及未完成项 |
| 视频与文字资料整理 | 保存允许下载的视频，整理标题、简介和来源，按主题归档 | 视频与文字对应表、来源清单、重复与失败记录 |
| 复杂脚本与批量处理 | 根据任务编写脚本，运行后检查结果；发现问题再修改 | 脚本、运行记录和结果文件 |
| 跨应用接续执行 | 将网页、安卓应用和本地文件中的资料汇总，再完成指定处理 | 可继续编辑的项目文件和交接说明 |
| 办公与研发资料处理 | 整理测试记录、核对需求版本、生成报告或演示材料 | 计算依据、差异清单及文档 |

应用版本、模型、操作权限和资料条件会影响任务完成情况。上表说明适用方向；具体任务先用少量样例确认操作和结果。小蓝不保证接手后每项任务都能完成。

## 工业工艺与研发应用

工艺与研发工作经常需要对照多版文件、整理试验记录，再根据任务要求处理数据、编写脚本或形成报告。小蓝可以参与这些需要跨资料、跨软件接续的工作，保留处理依据和可继续修改的成果，供工程人员检查。

小蓝助手已有多家制造业上市公司客户案例。企业可围绕自己的工艺资料、研发任务和现有流程咨询具体应用方式、本地化部署与技术支持。涉及工艺参数、设备操作、安全和产品性能的结论，由负责的专业人员审核确认。

## 从一个任务开始

1. 从[GitHub最新发行页](https://github.com/ffawei/xiaolan-assistant-bluedoai/releases/latest)或[官网工具与下载页](https://www.bluedoai.com/tools/)获取小蓝助手，按当前版本说明安装并配置模型。
2. 准备一个独立工作目录，放入可处理的资料，写清目标、输出格式和完成标准。
3. 授权所需的应用与目录；需要登录的应用先完成登录。
4. 让小蓝执行任务，检查输出文件；未完成项保留原因，再决定是否继续。

可以从这几份任务模板开始：

- [小蓝助手：视频与文字资料整理](examples/video-materials.md)
- [小蓝助手：Photoshop 图片处理](examples/photoshop-images.md)
- [小蓝助手：跨应用资料汇总](examples/cross-app-work.md)
- [小蓝助手与 MuMu：ADB 连接准备](docs/mumu-adb.md)

这些文件是可调整的任务模板，不是客户案例或已执行的成功报告。按自己的应用和资料填写后使用。

## 工具与模型费用

小蓝助手工具本体可免费使用，支持接入自有模型 API 或本地算力；接入方式与适用条件以当前客户端说明为准。需要托管模型时，可通过 BlueDoAI 管理模型接入、API Key 和用量，模型调用按实际用量计费。

可用模型及最终价格见[实时模型广场](https://www.bluedoai.com/model-plaza)。本地化部署、培训和专项技术服务按项目确定。

## 关于 MuMu、ADB 与 Photoshop

MuMu 在 Windows 上提供安卓运行环境，ADB 是小蓝连接和操作安卓环境的通道。这里的跨平台任务指 Windows 与 MuMu 中安卓应用之间的接续操作，具体见[连接指南](docs/mumu-adb.md)。

Photoshop 需要用户自行安装和合法使用。图片处理任务要写明尺寸、格式、参考效果和验收要求。MuMu、Android 与 Adobe Photoshop 的名称分别属于其权利人，提及这些产品不代表合作或背书。

## 使用与反馈

仅处理自己拥有或获得授权的文件与内容，遵守所使用应用的规则。下载采用应用允许的方式；需要登录、许可或人工确认时按提示完成。反馈问题时提供应用版本、脱敏任务步骤和错误信息，不公开 API Key、账号或客户资料。

本仓库提供小蓝助手 Blue（BlueDoAI）的产品介绍、接入文档和任务模板，不包含客户端源码。软件使用条件见[服务条款](https://www.bluedoai.com/legal/terms/)与[使用政策](https://www.bluedoai.com/legal/usage-policy/)。

官网：<https://www.bluedoai.com/>  
企业邮箱：<blue@bluedoai.com>
