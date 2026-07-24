# Security Policy

## Supported version

当前支持 Skill `0.5.3`，对应固定运行时 `vitalmcp@0.5.3`。

## Reporting a vulnerability

请优先使用 GitHub 的私有漏洞报告功能联系维护者。不要在公开 Issue、讨论区或聊天中披露以下内容：

- 配对二维码、深链或配对码；
- 私钥、令牌和 `~/.vital-agent-sync/secrets` 中的内容；
- SQLite 数据库、Apple Health 原始记录或健康报告；
- 包含上述内容的日志、截图或录屏。

报告中请提供不含敏感数据的复现步骤、预期行为、实际行为、macOS 与 WorkBuddy 版本，以及受影响的 Skill 和 `vitalmcp` 版本。

如果 GitHub 私有漏洞报告入口尚未启用，请先通过仓库所有者的 GitHub 个人资料联系维护者，不要创建包含漏洞细节的公开 Issue。

## Scope

本仓库只包含 WorkBuddy Skill。`vitalmcp` 运行时和 Vital Agent iOS App 的漏洞应在对应产品的安全渠道报告。
