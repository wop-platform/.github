# 万联易达开放平台 (WOP Platform) 👋

<div align="center">
<img src="https://raw.githubusercontent.com/wop-platform/.github/refs/heads/main/profile/logo_3x-black.BGQXcMOp.webp" alt="WOP Logo" width="600">

**万联易达开放平台 - 为开发者提供一站式数智化产业服务**

[![Website](https://img.shields.io/badge/Website-open.wanlianyida.com-blue)](https://open.wanlianyida.com)
[![Email](https://img.shields.io/badge/Email-contact@wlyd.com-red)](mailto:contact@wlyd.com)
[![License](https://img.shields.io/badge/License-Apache--2.0-green)](../LICENSE)
[![GitHub followers](https://img.shields.io/github/followers/wop-platform?style=social)](https://github.com/wop-platform)

**Languages:** [English](README.md) | [中文](#)
</div>

## 🙋‍♀️ 关于我们

万联易达开放平台（WOP Platform）是万联易达为开发者和企业提供的一站式数智化产业服务平台。万联易达是以生产性服务业平台运营为主业的产业互联网公司，通过线上平台与线下服务，提供覆盖全行业、全品类的一站式数智化综合性产业服务。我们致力于：

- 🚀 **简化服务集成**：提供简单易用的API和SDK，让产业服务集成变得轻松
- 🔒 **安全可靠**：以企业级安全标准保障每一次数据交互的安全
- 🌐 **多场景支持**：覆盖商品交易、物流仓储、数智金融、数字科技、人工智能、产业资讯、商务服务等全行业全品类场景
- 📱 **跨平台兼容**：支持多种编程语言和开发框架

## 🚀 快速开始

1. **注册账号** — 在[万联易达开放平台](https://open.wanlianyida.com)注册并创建应用
2. **选择 SDK** — 根据开发语言选择官方 SDK（见下表）
3. **开始开发** — 参考 [API 文档](https://open.wanlianyida.com/docs) 发起第一次调用

## 📜 公开规格

全部对外协议规格、SDK 统一规格与跨语言黄金测试向量集中在 [wop-specs](https://github.com/wop-platform/wop-specs)：

- [加密协议 Spec](https://github.com/wop-platform/wop-specs/blob/main/crypto/crypto-strategy-spec.md) — `securityReq` 算法套件、线上编码契约、协议不变式
- [SDK 统一规格](https://github.com/wop-platform/wop-specs/blob/main/sdk/wop-sdk-spec.md) — 各语言官方 SDK 的统一规格（v1.0-ratified）
- [黄金测试向量](https://github.com/wop-platform/wop-specs/blob/main/crypto/crypto-vectors.json) — 跨语言字节级一致性基准

## 🛠️ 核心产品

### SDK 开发工具包

我们为不同编程语言提供了官方SDK，让您快速集成平台服务能力：

| 语言 | 仓库 | Stars | 文档 | Channel |
| ------ | ------ | ----- | ------ | ------- |
| ☕ Java | [wop-java-sdk](https://github.com/wop-platform/wop-java-sdk) | ![Stars](https://img.shields.io/github/stars/wop-platform/wop-java-sdk) | [查看文档](https://github.com/wop-platform/wop-java-sdk#readme) | [Maven Central](https://central.sonatype.com/artifact/com.wanlianyida/wop-java-sdk) |
| 🐍 Python | [wop-python-sdk](https://github.com/wop-platform/wop-python-sdk) | ![Stars](https://img.shields.io/github/stars/wop-platform/wop-python-sdk) | [查看文档](https://github.com/wop-platform/wop-python-sdk#readme) | [PyPI](https://pypi.org/project/wop-python-sdk/) |
| 🟦 TypeScript | [wop-typescript-sdk](https://github.com/wop-platform/wop-typescript-sdk) | ![Stars](https://img.shields.io/github/stars/wop-platform/wop-typescript-sdk) | [查看文档](https://github.com/wop-platform/wop-typescript-sdk#readme) | [npm](https://www.npmjs.com/package/@wanlianyida/wop-typescript-sdk) |
| 🐘 PHP | [wop-php-sdk](https://github.com/wop-platform/wop-php-sdk) | ![Stars](https://img.shields.io/github/stars/wop-platform/wop-php-sdk) | [查看文档](https://github.com/wop-platform/wop-php-sdk#readme) | [Packagist](https://packagist.org/packages/wop-platform/wop-php-sdk) |
| 🔷 .Net | [wop-dotnet-sdk](https://github.com/wop-platform/wop-dotnet-sdk) | ![Stars](https://img.shields.io/github/stars/wop-platform/wop-dotnet-sdk) | [查看文档](https://github.com/wop-platform/wop-dotnet-sdk#readme) | [NuGet](https://www.nuget.org/packages/Wop.Sdk/) |
| 🐹 Go | [wop-go-sdk](https://github.com/wop-platform/wop-go-sdk) | ![Stars](https://img.shields.io/github/stars/wop-platform/wop-go-sdk) | [查看文档](https://github.com/wop-platform/wop-go-sdk#readme) | [Go](https://pkg.go.dev/github.com/wop-platform/wop-go-sdk) |

### 在线工具

- 🧰 [WOP Web Tools](https://github.com/wop-platform/wop-web-tools) — 浏览器端商户工作台：密钥生成、报文联调、离线验证。纯静态单文件，密钥本地生成、零上传。

### Agent

WOP 开放平台官方 Agent 能力——当前提供技能包，MCP 工具等持续扩展——让每一个商户 Agent 安全、正确地完成 API 对接。

- 🤖 [wop-skills](https://github.com/wop-platform/wop-skills) — 零代码 API 对接技能包：wop-cli（签名→调用→验签）、wop-dev（协议心智模型）、wop-troubleshoot（62 错误码排错） ![Tests](https://img.shields.io/badge/tests-73%20passed-brightgreen) ![Coverage](https://img.shields.io/badge/line%20coverage-97%25-brightgreen) ![Stars](https://img.shields.io/github/stars/wop-platform/wop-skills)

### 示例项目

- 🤖 [WOP MCP](https://github.com/wop-platform/wop-mcp)

## 🌈 如何参与贡献

我们欢迎社区的每一份贡献！您可以通过以下方式参与：

### 💡 贡献代码

1. **Fork** 相应的仓库
2. **创建** 您的功能分支 (`git checkout -b feature/AmazingFeature`)
3. **提交** 您的更改 (`git commit -m 'Add some AmazingFeature'`)
4. **推送** 到分支 (`git push origin feature/AmazingFeature`)
5. **创建** Pull Request

### 🐛 报告问题

- 在相应仓库的 Issues 页面报告 bug
- 提供详细的复现步骤和环境信息
- 建议改进和新功能

### 📖 完善文档

- 改进现有文档
- 翻译文档到其他语言
- 分享使用经验和最佳实践

## 👩‍💻 有用资源

### 📚 官方文档

- 🌐 [万联易达开放平台官网](https://open.wanlianyida.com)
- 📖 [API 文档](https://open.wanlianyida.com/docs)
- 🔧 [开发者工具](https://open.wanlianyida.com/tools)

### 🆘 获取帮助

- 📧 **技术支持**：[contact@wlyd.com](mailto:contact@wlyd.com)
- 💬 **社区讨论**：在相应仓库的 Discussions 区域
- 📞 **商务合作**：访问官网联系我们

### 🔗 相关链接

- [万联易达官网](https://www.wanlianyida.com)
- [开发者社区](https://open.wanlianyida.com/community)
- [API 状态页面](https://status.wanlianyida.com)

## 🍿 团队趣事

- ☕ **早餐选择**：我们团队成员遍布全国，有人喜欢豆浆油条，有人钟爱咖啡面包，但大家都对代码质量有着同样的执着！
- 🎯 **代码审查**：我们相信"代码如诗"，每次代码审查都像是在品味一首技术诗歌
- 🚀 **持续改进**：我们的座右铭是"以科技重塑产业协作"，每个功能都经过精心打磨

## 📄 开源协议

大部分项目采用 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0) 和 [MIT License](https://opensource.org/licenses/MIT) 开源协议。

---

<div align="center">
<p>
  <strong>构建覆盖全产业、全场景、全链路的智能服务网络</strong><br>
  Made with ❤️ by WOP Platform Team
</p>

[![Follow](https://img.shields.io/github/followers/wop-platform?style=social)](https://github.com/wop-platform)
[![Star](https://img.shields.io/github/stars/wop-platform?style=social)](https://github.com/wop-platform)
</div>
