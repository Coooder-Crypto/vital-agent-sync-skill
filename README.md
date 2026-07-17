# Vital Agent Sync Skill

面向 WorkBuddy 的开源安装与使用 Skill。它引导 WorkBuddy 安装固定版本的 `vitalmcp` 本地运行时、配置 MCP、启动本地服务，并在 Mac 上打开供 iPhone 扫描的配对二维码。

## 一句话开始

安装本 Skill 后，在 WorkBuddy 中发送：

> 请安装 Vital Agent Sync，使用局域网模式连接我的 iPhone。先说明会进行哪些持久化修改，等我确认后执行，最后在本机打开配对二维码。

Skill 会先展示安装计划并请求确认，不会静默修改本地配置。

## 环境要求

- macOS；
- Node.js 22 或更高版本及 npm；
- 安装了 Vital Agent 的 iPhone；
- Mac 与 iPhone 位于可互相访问的可信局域网；
- WorkBuddy。

## 安装方式

在 SkillHub 上架后，优先从 SkillHub 一键安装。开发和审核期间，也可以在 WorkBuddy 的 Skills 页面中导入本仓库根目录的 `SKILL.md`。

本 Skill 当前固定安装公开 npm 包 `vitalmcp@0.5.1`，不会使用 `sudo`，也不会执行来源不明的远程脚本。

## 仓库边界

本仓库只开源 WorkBuddy Skill，即 Agent 可审阅的安装、配对、调用和安全策略，不包含：

- Vital Agent iOS App 源代码；
- `vitalmcp` 运行时源代码；
- Apple Health 数据、数据库、二维码、配对令牌或其他用户凭据。

本仓库代码采用 MIT License。Vital Agent Sync 的产品名称、Logo 和其他品牌资产不因该许可证自动获得授权。

## 隐私与安全

健康数据库和同步运行时默认保留在用户 Mac 上。WorkBuddy 调用 MCP 后，为回答问题而返回的必要健康上下文可能会发送给用户选择的模型提供商。请只授权所需的数据，并检查所选模型服务的隐私条款。

Vital Agent Sync 是用户控制的数据网关，不是医疗服务，不提供诊断、治疗或急救建议。

发布安全问题前请阅读 [SECURITY.md](SECURITY.md)。不要在公开 Issue 中粘贴二维码、深链、配对码、令牌、数据库或健康数据。

## 版本关系

Skill 版本与其固定的 `vitalmcp` 版本保持一致。当前版本为 `0.5.1`。
