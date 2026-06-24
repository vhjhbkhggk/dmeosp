# MQSAQL Reference Index

MQSAQL Reference Index 是一个面向数据库技术研究与工程实践的集中式外链资源汇总站。项目定位于收集、整理并持久化与 MQSAQL 相关的技术文档、案例分析、性能调优记录以及社区讨论的快照链接，为数据库内核开发者、SRE 工程师以及数据中间件维护人员提供可追溯的原始材料参考。

本项目不提供代码实现或运行时二进制，而是围绕特定批次的原始数据快照构建索引目录，帮助用户在复杂的代码仓与碎片化记录中快速定位到与 MQSAQL 相关的具体提交、讨论或变更历史。每一份被收录的链接均指向 GitHub 仓库中的永久性 Markdown 记录，确保引用的稳定性和可验证性。

## 功能概览

- **按批次索引**：将大量外部分散链接按批次分组，当前为第 44/114 批，便于用户理解数据规模与进度。
- **原始内容直链**：每个收录项直接指向原始 GitHub 服务器上的 Markdown 文件，不经过任何代理或中间页跳转，保证访问路径最短。
- **主题标签分类**：在资源列表中根据文件名哈希前缀和内容上下文自动归入技术子主题，如查询优化、存储引擎、事务日志等。
- **结构化元数据**：每个链接附带所在仓库路径、文件名哈希及提交上下文，便于与 Git 历史对照。
- **版本化快照引用**：所有链接指向固定分支 main 下的稳定路径，避免因分支演进导致的链接失效。
- **快速目录跳转**：提供清晰的章节内锚点与表格导航，用户可在数秒内从概览直达具体资源分组。
- **兼容离线阅读**：项目结构及资源列表以纯 Markdown 撰写，支持克隆到本地后使用任何文本编辑器离线浏览。
- **持续更新追踪**：通过批次号标识当前进度，后续批次将在同一结构中追加，保持整体组织一致性。

## 应用场景

- **数据库内核问题回溯**：当线上环境出现与 MQSAQL 相关的异常行为时，工程师可以快速翻阅本索引中对应的历史分析记录，比对当前行为与过往快照的差异。
- **性能基准测试参考**：在进行版本升级或配置变更前，团队可通过索引中的链接获取先前性能测试的原始数据记录，作为调优基准。
- **新成员技术学习路径**：新加入团队的数据库开发人员可通过本索引按批次顺序浏览技术文档，逐步建立对项目演进脉络和关键变更的认知。
- **技术报告与审计材料引用**：技术负责人或合规审计人员可将本索引中收录的公开链接作为报告附件，确保引用来源清晰、可复现。
- **社区贡献前调研**：外部贡献者在提交代码或文档之前，可查阅本索引以确认是否已有类似讨论或记录，避免重复劳动。

## 快速开始

以下操作适用于首次使用本项目的用户，需确保本地环境已安装 Git 及任意 Markdown 阅读器。

```bash
# 克隆项目仓库
git clone https://github.com/vhjhbkhggk/mqsaql.git

# 进入项目目录
cd mqsaql

# 使用任意 Markdown 预览工具打开 README.md
# 例如使用 vscode 内置预览，或命令行工具如 glow、mdless
glow README.md
```

## 安装要求

本项目仅为文档索引，无需安装额外依赖。但若用户希望完整离线浏览所有引用的 Markdown 文件，建议确保本地网络可访问 GitHub 原始内容域名。以下列出推荐的基础环境：

| 依赖 | 必需 | 说明 |
|------|------|------|
| Git | 是 | 用于克隆仓库及后续拉取更新 |
| Markdown 阅读器 | 是 | 本地预览 README 及索引内容 |
| 网络连接 | 推荐 | 用于访问外部链接中的原始文件内容 |
| 命令行环境 | 否 | 非必需，但便于执行 git 命令和脚本 |
| Python 3.6+ | 否 | 仅用于运行可选的链接有效性检查脚本 |
| curl 或 wget | 否 | 用于批量下载参考文件做离线备份 |

## 文档导航

| 层面 | 目录 | 回答的问题 |
|------|------|------------|
| 项目总览 | 项目名、简介、功能概览 | 该项目是什么，包含哪些核心能力 |
| 使用指南 | 快速开始、安装要求 | 如何获取项目、如何本地浏览 |
| 资源索引 | 资源列表 | 具体收录了哪些外部链接，如何分类 |
| 工程管理 | 项目结构、贡献指南、常见问题 | 目录如何组织、如何参与、常见疑问 |

## 资源列表

### 第 44 批核心索引文件

https://github.com/vhjhbkhggk/mqsaql/blob/main/6edb6ce3f4926447.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6edf2d951ef7b959.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6ef0548d91f34b6a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6f1d5eba61a956f5.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6f41a8942331822b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6f668be15b8f742d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6f7ee9d7fe25c2a7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6f94c2ef67fe6f56.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6fd72bce4954817b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6fdc24ad0909a055.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6fe3faa920cb0f19.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/6ff1d6079b39688d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/702705a91fd1489a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/70fda8243985fe11.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/71093d532a67a486.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/710ae8e847ddb337.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/711fd27adc1e4dd7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7128ac2422dfa6a3.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/716f6248406a7497.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7253b9f720bf5555.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/72892193304bc933.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/729ee9d7a8d3d239.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/72a8d90891253b8b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/72ef72700e6f4bab.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/72f28e0ddf2b3a55.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/72ffb05884edf12e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/733db1295aacc053.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7351f4f454eac32c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/73a249b349f3f3dd.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/73a54a2dd3ed4545.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/73d36e8a0511e308.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/73eaa8498809d117.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/73f50ee8dd44368b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/73f64faf2956109d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/73f6abd50b45094d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/73fcb3955efb836c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/74461c5d357b9704.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/74508242da9c3aed.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/749adf0157671bdc.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/74d737ba5b35567a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/754e77f8f33e4f4f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/75bb42197ed8fc28.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/75e3bd68f07ea19d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/75ea35db1ca143c1.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/76247c37469aa176.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/76417ca5e8103f30.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/765043159b4876b8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7681c01b6f4910d6.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/76999e5aa0c0427e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/769b2f1b5df88506.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/76c0e963cf6d8bda.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/77316e6c7eb057ac.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/774a25bc6234ec54.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/774ced76717c8564.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/776717351801da3d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/77a399b3e8e14715.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/77aa55dcff5696eb.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/77cd1f12a534f1c4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/77d6021675e267ae.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/77e2cc17b5a2e8ad.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/77e8007ddd9f6835.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/77ec203638d31134.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/78047d24c56be498.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7808cff6ce9e7a4b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/780a57a77637aed0.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/781f293239b7e1b0.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7846b4b01b24c5f0.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7856c8d502705921.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/78594c95fda99549.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/78aa49ca68ad4dfb.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/78bb03caf93262fb.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/78d2c119f74a60a5.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/78ec1027c4ae26cd.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/79311f1dbbcfb52c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/79371b9bbf0c73fa.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7972b9ac754cf9ef.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/79b2da66a0c8e8a7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/79b7aba534bc3459.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/79ba8a54d9875fa4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/79cbfed3db2a7ab2.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/79d720749c4fb161.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/79f00afed658dbd4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/79f0c8c53c1b5f4c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a02e4753cbda822.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a20ccb60d3d2c9e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a3062625853a41d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a4e7ec8091e3f0e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a682e6d5ea54d12.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a6e4f5b7043e8b9.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a7fb35dcccee2d6.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a8af01b269ce429.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a8c653fad42bec5.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a918c3e3640a337.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7a9f4c5cc280eeab.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7aaf3d2ff5a71f12.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7ab14ce83636c8a5.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7abfd5fd6fc4b930.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7af225d37e46022e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b133ebd0348b584.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b1906c1a98714ac.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b1fdd81ed73e118.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b259e5fc6dfa356.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b4141cd293fbe5b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b417d37494b7d7f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b46a02df9889661.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b570b8129ef24b4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b5c23eb9bd0546d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7b7519fe992dfdff.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7bc415a326988fe2.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7be7cebd1dd65a90.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7c0916c522344207.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7c1d053f52dae8e0.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7c2d8ac4fd3fa040.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7c4fd37b75b4f145.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7c8c42ad635aeb5c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7cb8dbf822cf4b89.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7ce7cd48f2d046d5.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7ceb2bae2a8c051b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7cf41367632ab299.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7cfc658cc2c69239.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7d0b60bbcaed9272.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7d0fbcc521c4dc2b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7d84813771666d26.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7d8c05322366d579.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7d92d8a77bc80900.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7dab93d89c1941c2.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7dba21a14e803296.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7dbdf3417ddaab22.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7dde8c0e0cc35634.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7e041ce101517169.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7e12d4b28b0de968.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7e15f8e8be927c23.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7e227c7715096e29.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7e84ce1b3e918d3f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7e8faf28a220f1bc.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7e9177adda8d2e6d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7e973d11cf7690e7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7e9cfc2eb5280fac.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7ea85269f743e553.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7efec193b315ba19.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7f0d48709a8eae18.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7f1b41e7bfae82bd.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7f4a217cce1d9421.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7f62829a92035591.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7fac1669fd02f30b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7fae4fe6ce26c2a0.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7fb0241ee0f63479.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7fb49ee95ecdabf1.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7fbad57e799a0cd9.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7fbd02b13bbdd974.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/7fcac773e227198b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/804e9d9431122af6.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/805883498a02a151.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/80621d2bef9a0594.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/80931e7865f458eb.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8099c566f3591a54.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/80a0e139fc1417b5.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/80a57963539d9361.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/80ac2d92d80c1091.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/80e3c787495e7f8d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/80f6209d4c7b7d0e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8102e73679e8b5c9.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/810dc464c27d3aa7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8151692738fc6c42.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8155836290fb8c04.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/816cea70e9b1526c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/81880422698e9e82.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/81c6864c7b1a926d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/81dd306cc9264ca5.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/820ecc20aab0f816.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/821247ff6bdffce1.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8239efa91019d424.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/824fb425b6f1db06.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/828ae32e78d52a32.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/82b55fc79d9b195d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/82e8b471738cdf9e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/82ea0d36ff91aee7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/82eb14267ba2ea00.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/82f5196a0caf5445.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/83087097a68e40c6.md

## 项目结构

```
mqsaql/
├── README.md                         # 项目总览与索引入口
├── main/                             # 主要资源分支目录
│   ├── 6edb6ce3f4926447.md           # 第44批资源文件 1/180
│   ├── 6edf2d951ef7b959.md           # 第44批资源文件 2/180
│   ├── ...                           # 其余 178 个哈希命名文件
│   └── 83087097a68e40c6.md           # 第44批资源文件 180/180
├── scripts/                          # 辅助工具脚本目录
│   ├── link_validator.py             # 批量检查收录链接可访问性
│   └── index_generator.sh            # 根据文件列表自动生成索引表格
├── archive/                          # 历史批次归档目录
│   ├── batch_43/                     # 上一批次完整索引副本
│   └── batch_42/                     # 更早期批次存档
├── docs/                             # 项目自身文档目录
│   ├── contribution_guide.md         # 详细贡献者操作手册
│   └── url_maintenance_policy.md     # 链接更新与淘汰策略说明
└── templates/                        # Markdown 模板目录
    └── resource_template.md          # 新增资源文件的推荐格式模板
```

## 贡献指南

1. 检查现有资源列表以避免重复收录。若发现重复或失效链接，请先在 issue 中提出并说明理由。
2. 新增外部链接时，需按照 templates/resource_template.md 中的格式填写标题、来源日期、简要摘要和原始 URL，并放置于 main/ 目录下以哈希命名。
3. 修改资源分类或调整索引结构前，请先在本地运行 scripts/index_generator.sh 验证索引表格的完整性，确保不破坏现有章节锚点。
4. 提交 pull request 时请附上变更说明，包括新增链接的简要背景、修改目的以及本地自测结果（如运行 link_validator.py 的输出摘要）。
5. 若遇到链接原始仓库发生迁移或删除，请及时在 issue 中标记，并将对应条目移至 archive/ 目录下，同时在 README 中更新状态注释。

## 常见问题

问：本项目是否提供对 MQSAQL 源代码的直接修改或补丁支持？

答：不提供。本项目仅为外链索引和资源汇总，不托管任何源代码实现或二进制制品。所有指向的内容均位于外部 GitHub 仓库中，本项目仅做引用和分类。

问：如果某个收录的链接失效或内容被移除，应该如何处理？

答：请先在源仓库中确认文件是否被重命名或移至其他分支。若确认已彻底移除，可提交 issue 通知维护者，维护者将把对应条目移至 archive/ 并添加失效标记，但不会删除其记录以保留历史引用脉络。

问：新批次资源何时更新，如何跟踪进度？

答：本项目按批次推进，当前为第 44/114 批。后续批次会在当前结构下扩展资源列表，并更新章节首部的批次信息。用户可通过定期 git pull 获取更新，或关注仓库的 release 标签获取稳定版本快照。

## 许可证

MIT

> 外链数量: 180 | 生成时间: 2026-06-24 18:30:06
