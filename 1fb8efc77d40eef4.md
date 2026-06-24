# ResourceBridge

ResourceBridge 是一个面向开发者与技术研究人员的结构化外链与资源聚合工具。该项目不对资源内容进行二次编辑或镜像存储，而是通过严格的分类索引、标签化元数据和可检索的目录结构，将分散于各大社区、代码托管平台及技术博客中的优质外部链接进行系统化整理。ResourceBridge 的目标用户包括技术文档撰写者、开源项目维护者、技术选型评估人员以及持续跟踪行业动态的研发工程师。该项目解决了技术资源发现效率低、信息孤岛严重、书签管理混乱且缺乏上下文关联等核心问题，通过将外部链接与项目内 Markdown 说明文档进行绑定，使得每一条外链都具备可追溯的收录理由、适用场景和版本适配信息。

## 功能概览

**批量外链导入与哈希索引**：支持通过脚本或 API 将大批量 URL 导入系统，自动计算短哈希作为存储键值，避免重复收录。

**多级目录分类存储**：所有外链按照技术领域、资源类型和时效性三个维度被归类至不同的子目录，目录层级可自定义扩展。

**Markdown 元数据增强**：每个外链对应的 Markdown 文件均包含 YAML Front Matter 头部字段，记录收录时间、标签列表、原始来源域名和推荐指数。

**全文检索与过滤**：基于文件名哈希和元数据字段实现快速定位，支持按域名、文件扩展名、关键词组合进行过滤。

**链接可用性监控**：内置定时任务对已收录链接进行 HTTP 状态检查，自动标记失效链接并生成报告。

**项目内交叉引用**：允许在不同资源文件之间建立双向引用关系，形成知识网络而非扁平列表。

**导入导出标准化**：支持将资源列表导出为 JSON、CSV 或纯文本格式，便于与其他工具链集成。

## 应用场景

**技术选型调研**：当团队需要评估多个开源库或云服务时，可以通过 ResourceBridge 快速查阅已收录的第三方评测链接、官方文档和社区讨论，避免重复搜索。

**文档站外链管理**：技术文档撰写者可以在编写教程或 API 参考时，将需要引用的外部资料通过 ResourceBridge 统一托管引用，确保链接变更时可集中更新。

**团队知识库构建**：研发团队可将日常积累的故障排查帖子、性能优化案例和架构设计参考链接全部录入 ResourceBridge，配合元数据标签形成可共享的团队知识资产。

**开源项目依赖跟踪**：对于依赖大量上游项目的开源仓库，可以使用 ResourceBridge 记录每个依赖项的官方地址、迁移公告和废弃状态，降低维护风险。

## 快速开始

```bash
git clone https://github.com/your-org/resource-bridge.git
cd resource-bridge
pip install -r requirements.txt
python scripts/ingest.py --input ./urls.txt --output ./resources
```

上述命令会从 urls.txt 文件中读取 URL 列表，对每个 URL 计算哈希值并生成对应的 Markdown 存根文件，存放于 resources 目录下。若需启动本地 Web 界面进行可视化管理，可执行 python app.py 并访问本地端口。

## 安装要求

| 依赖组件 | 必需版本 | 说明 |
|---|---|---|
| Python | 3.9 及以上 | 核心脚本运行环境，负责链接处理与元数据生成 |
| Git | 2.30 及以上 | 用于克隆仓库及版本管理 |
| pip | 22.0 及以上 | Python 包依赖管理工具 |
| requests | 2.28.0 及以上 | 发送 HTTP 请求进行链接可用性检查 |
| pyyaml | 6.0 及以上 | 解析和生成 Markdown 文件的 YAML Front Matter |
| markdown | 3.4.0 及以上 | 可选依赖，用于将 Markdown 渲染为 HTML 预览 |
| sqlite3 | 3.35 及以上 | 本地缓存与检索索引的数据库引擎 |
| cron | 系统自带 | 用于定时执行链接监控任务（Linux/macOS） |

## 文档导航

| 层面 | 目录 | 回答的问题 |
|---|---|---|
| 入门指南 | docs/getting-started.md | 如何安装、配置首次运行、理解核心概念与目录结构 |
| 链接收录规范 | docs/link-policy.md | 什么样的链接可以被收录、元数据字段填写规则、标签命名约定 |
| 运维手册 | docs/operations.md | 如何执行批量导入、如何更新失效链接、如何备份资源索引 |
| 高级定制 | docs/advanced/custom-parser.md | 如何编写自定义解析器以支持非标准 URL 格式或第三方平台特有链接 |

## 资源列表

### 第 19 批资源（共 180 个链接）

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
https://github.com/vhjhbkhggk/mqsaql/blob/main/8320fdac14265827.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8325512e6c790a88.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8342e561a3293dd8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/83506d39ec638cb8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/83593e7e5718e9ae.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8361001af8fd52c9.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8395bfb2c8c4542a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/83a036b7d2ee9909.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/83aeea70acf04001.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8406bdd2f53f96dd.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8408ecf22770a472.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/840c348f05fb867c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/84206d41a8543d40.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/8441345d0aaba8f0.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/845e30cbdccde805.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/84a0fae997d0cb26.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/84a322c79075780b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/84bf142a18af7fd7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/84ce73307919e7e8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/84ff258610fc7033.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/850962b94389d079.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/851730f913691000.md

## 项目结构

```
resource-bridge/
├── app.py                           # Web 管理界面主程序，基于 Flask
├── config.yaml                      # 全局配置文件，包含存储路径、监控间隔等
├── requirements.txt                 # Python 依赖声明
├── scripts/                         # 可执行脚本目录
│   ├── ingest.py                    # 批量导入外链的核心脚本
│   ├── check_links.py               # 链接可用性检查脚本
│   └── export.py                    # 资源列表导出工具
├── resources/                       # 外链存储根目录，按哈希组织
│   ├── 72/                          # 哈希前两位作为一级目录
│   │   ├── 72a8d90891253b8b.md      # 每个链接对应一个 Markdown 文件
│   │   └── 72ef72700e6f4bab.md
│   ├── 73/                          # 第二批哈希目录
│   │   ├── 73a249b349f3f3dd.md
│   │   └── ...
│   ├── 80/                          # 后续哈希目录类推
│   │   ├── 804e9d9431122af6.md
│   │   └── ...
│   └── index.db                     # SQLite 索引数据库，缓存元数据
├── docs/                            # 项目文档目录
│   ├── getting-started.md
│   ├── link-policy.md
│   ├── operations.md
│   └── advanced/
│       └── custom-parser.md
├── tests/                           # 单元测试目录
│   ├── test_ingest.py
│   └── test_check_links.py
└── templates/                       # Web 界面模板文件
    ├── index.html
    └── detail.html
```

## 贡献指南

1. 在 GitHub 上 Fork 本仓库，并在本地克隆您的 Fork 版本。请确保您的开发分支基于 main 分支的最新提交。

2. 新增外链资源时，请先查阅 docs/link-policy.md 中的收录规范，确保链接内容与现有分类体系一致。若引入新的技术领域标签，需同步更新 config.yaml 中的标签白名单。

3. 提交代码或资源变更前，请运行 scripts/check_links.py 对新增或修改的链接进行可用性验证，并确保所有单元测试通过（执行 pytest tests/）。

4. 提交 Pull Request 时，请在描述中清晰说明本次变更的目的、涉及的链接数量以及是否影响现有索引结构。PR 至少需要一名维护者审核通过后方可合并。

## 常见问题

**问：ResourceBridge 是否会存储外部链接的内容副本？**

答：不会。ResourceBridge 仅存储链接自身的元数据（如标题、标签、收录时间）以及可选的摘要描述。所有实际内容均通过原始 URL 访问，项目不承担任何内容分发或缓存职责。

**问：如何处理收录链接失效或内容变更的情况？**

答：项目内置了定时检查机制，每日自动扫描所有已收录链接的 HTTP 状态码。对于返回 4xx 或 5xx 的链接，系统会将其标记为失效并在 Web 界面中高亮显示。维护者可以手动确认后更新链接地址或移除该条目。

**问：能否将 ResourceBridge 与我现有的静态站点生成器集成？**

答：可以。scripts/export.py 支持将资源列表导出为 JSON 或 CSV 格式，您可以编写自定义脚本将其转换为 Hugo、Jekyll 或 VuePress 等工具所需的数据格式。项目本身不强制绑定任何前端框架。

## 许可证

MIT

> 外链数量: 180 | 生成时间: 2026-06-24 18:30:06
