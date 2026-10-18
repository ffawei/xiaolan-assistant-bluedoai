# 产品 FAQ 与常用答复

**BlueDoAI 提供什么？**  
提供 AI 模型与算力接入，统一管理 API Key、余额和用量。当前型号与价格见 https://www.bluedoai.com/model-plaza 。

**小蓝助手能做什么？**  
在授权范围内处理工艺与研发资料、编写和运行复杂脚本、参与 PS 图片处理，在支持的应用之间接续执行，交付可复核文件。介绍：https://www.bluedoai.com/legal/product-overview/ 。

**工具是否收费？**  
工具本体免费。自有模型 API 按相应服务方规则结算；BlueDoAI 托管模型按量计费；企业部署、定制等专项服务单独约定。https://www.bluedoai.com/legal/billing/ 。

**能否接自己的 API 或本地算力？**  
支持自有模型 API；兼容本地模型服务的接口、版本与功能适配需按当前客户端说明核对。不能将“支持本地模型”理解为所有版本、所有模型都完整适用。

**API 怎样接？**  
选择分组、创建 API Key，按接入页设置 Base URL 和模型名。文本入口为 https://api.bluedoai.com/v1 。复制模型广场的 API 名称，例如 glm-5.2；模型必须在该 Key 所属分组中可用。https://www.bluedoai.com/api-access/ 。

**视频模型可以用聊天接口调用吗？**  
视频按对应异步任务接口提交、查询和获取结果，不按文本聊天接口使用。具体型号、规格与计费以模型广场和接口说明为准。

**企业能否本地化部署？**  
可以围绕企业资料、岗位和流程协商实施方案。部署组件、模型来源、权限、服务周期和验收标准按项目确认。https://www.bluedoai.com/enterprise/ 。

**本地部署是否意味着数据不离开企业？**  
需要看实际模型与网络配置。若调用外部模型，相关请求可能传往外部服务；完全本地的要求需单独设计和验收，不能仅凭助手本地安装作出承诺。

**企业折扣如何确定？**  
按具体模型、分组、会员授权和有效合同确定，以账户生效价格为准。不能把一个型号的折扣套用于全平台。

**从哪里下载？**  
官网提供 GitCode 国内下载和 GitHub 下载入口：https://www.bluedoai.com/tools/ 。GitHub 最新发行页：https://github.com/ffawei/xiaolan-assistant-bluedoai/releases/latest 。Windows 用户下载 .exe 安装程序。

**如何咨询合作？**  
企业邮箱 blue@bluedoai.com；微信 yikaoka；QQ 759508。https://www.bluedoai.com/contact/ 。

**有制造业客户案例吗？**  
小蓝助手已有多家制造业上市公司客户案例。企业可围绕工艺资料、研发任务和现有流程咨询具体应用方式：https://www.bluedoai.com/enterprise/ 。

**工业工艺与研发工作怎样开始？**  
选择一项具体任务，例如整理工艺文件、分析试验记录或核对需求版本。准备原始资料、已有计算规则和交付要求，让小蓝处理资料并留下来源与脚本，工程人员据此复核专业结论。

**能操作 PS 吗？**  
可以结合实际软件环境开展 Photoshop 图片处理任务。用户准备已安装的软件、素材、尺寸和输出要求，先确认当前版本与操作方式适用，再检查图片和可编辑文件。

**怎样结合 MuMu 处理安卓应用？**  
通过 ADB 连接指定的 MuMu 实例，在授权范围内操作支持的安卓应用，再把资料交到 Windows 端继续处理。连接准备见 https://github.com/ffawei/xiaolan-assistant-bluedoai/blob/main/docs/mumu-adb.md 。

**可以先拿一项任务试用吗？**  
可以。先准备少量样例，写明完成标准，检查结果后再扩大范围。任务模板见 https://github.com/ffawei/xiaolan-assistant-bluedoai 。
