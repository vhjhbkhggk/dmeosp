# LinkVault Resource Aggregator

LinkVault Resource Aggregator 是一个面向开发者与技术研究人员的结构化外链与文档资源汇总工具。该项目不对托管内容进行二次加工，而是通过对海量外部参考文档、技术笔记与配置片段进行按需索引与分类整理，帮助用户快速定位所需信息。项目本身不提供数据库或后端服务，完全基于静态 Markdown 与可解析的链接清单运行，适用于个人知识库辅助、团队技术栈速查以及自动化文档流程的输入源。

本项目聚焦于解决以下问题：技术资料分散在多处、参考链接缺乏统一入口、碎片化笔记难以检索。LinkVault 将来自社区仓库的大量参考条目统一组织为可读、可扩展的清单结构，并保持原始来源的完整可追溯性。

## 功能概览

**按批次索引的链接目录** 项目将全部外链按来源批次与入库时间进行分段管理，每批条目对应一个独立章节，便于版本追溯与增量更新。

**原始链接直出模式** 所有收录的 URL 均保留用户提供的原始格式，不添加协议前缀、不修改域名大小写、不追加尾部斜杠，确保引用路径与源仓库完全一致。

**多维度分类视图** 资源列表按照技术领域、文件类型或用途进行二级分类，每个分类下集中展示相关链接，降低用户在大列表中的筛选成本。

**纯静态可移植结构** 项目不依赖动态运行时环境，所有数据均以 Markdown 表格与列表形式存储，可直接挂载至 GitHub Pages、内部 Wiki 或本地文件系统。

**与自动化工具兼容** 目录树与链接清单采用严格的格式规范，可被 Shell 脚本、Python 解析器或 CI 流程直接读取，用于生成导航页或执行链接有效性检查。

**文档结构自描述** 每个章节均配有明确的用途说明与字段定义，新贡献者可在无额外文档的情况下理解组织逻辑。

## 应用场景

**技术团队内部知识库的导航入口** 团队可将本项目作为索引层，将分散在 GitHub 仓库、技术博客与官方文档中的参考链接统一收录，新成员通过浏览目录即可了解常用资源分布。

**个人开发者的参考手册辅助工具** 开发者可在日常研究中将发现的有用外链按批次追加至项目清单，配合快速开始中的脚本生成本地可检索的 HTML 概览，减少重复搜索时间。

**文档自动化流程的数据源** 项目输出的纯结构列表可作为 CI 任务的输入，用于生成站点地图、做链接失效检测或按分类统计资源热度，无需额外解析复杂配置。

**开源社区的资源共建基础** 社区维护者可通过贡献指南向项目提交新批次链接，经审核后合并，形成众包式技术外链集合，降低个人维护海量书签的成本。

## 快速开始

以下步骤演示如何获取项目副本、安装必要工具并生成本地索引概览。

```bash
git clone https://github.com/your-org/linkvault.git
cd linkvault

# 安装依赖（用于本地预览与链接格式检查）
npm install -g markdown-link-check
pip install linkchecker

# 运行索引生成脚本（输出 resource_index.md）
./scripts/build_index.sh
```

执行完毕后，打开生成的 resource_index.md 即可查看全部链接的分类清单。若需启动本地预览服务器，可运行 `python -m http.server 8000` 并在浏览器访问对应地址。

## 安装要求

| 依赖 | 必需 | 说明 |
|------|------|------|
| Git | 是 | 用于克隆仓库及版本管理，推荐 2.25 及以上版本 |
| Node.js | 否 | 仅在使用 markdown-link-check 进行链接校验时需要，推荐 14.x 或更高 |
| Python 3 | 否 | 运行内置简易 HTTP 服务器或解析脚本时的可选运行时 |
| make | 否 | 若使用 Makefile 中的自动化任务（如 build、check）则需要 |
| curl | 否 | 用于从远程拉取外部资源清单的辅助工具，推荐 7.68 以上 |
| markdown-link-check | 否 | 全局安装的 npm 包，用于检测文档中的失效链接 |
| linkchecker | 否 | Python 环境下的链接检查工具，可作为备选方案 |

## 文档导航

| 层面 | 目录 | 回答的问题 |
|------|------|------------|
| 项目概览 | README.md | 项目定位是什么、包含哪些内容、如何使用 |
| 资源索引 | docs/resource_list.md | 全部外链按批次与分类的完整列表 |
| 贡献指引 | CONTRIBUTING.md | 如何新增链接、如何提交批次、审核标准是什么 |
| 版本记录 | CHANGELOG.md | 每个版本新增或移除了哪些资源、结构有何变动 |

## 资源列表

以下为第 77/114 批收录的全部原始链接，按入库文件名排序。所有链接均按用户提供的格式原样输出，未做任何修改。

技术参考文档类

https://github.com/vhjhbkhggk/mqsaql/blob/main/0d5a39dbdf3771a7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0df3962098c931e3.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0df8725e0e3ec932.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0e1663e5720d7749.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0e6304fac5022396.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0e8db5b5f14ee2d2.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0e9fb1ac6158a0db.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0eaab08f44e6c532.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0eb029627e451751.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0ebfbd1959ba1cd7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0ed084b81f4bd0f8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0ef2fa04e349ad4e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0ef4350ec626dafe.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0efa6f4f6852d196.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0f07ee1f63ebf46a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0f157f5beb701c75.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0f1a838717758d5c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0f1c23259f86c215.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0f7843da7821a94a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0f7dde613c176c22.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0f9e26ea10d8cab7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0fbf3f3f0552a22d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/0fd34fb2ab1bf105.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/10247f3576e274ef.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/10252480147c9870.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/104c12037073655c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1096633d085d12e8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1099f1844a66f777.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/10a6b5700e324684.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/10c7e8e0848b5982.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/10ecf3b1c49da771.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/10f18a9557eb9de7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/10f9d969f696a93d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/111b1512cb6a9cfa.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/115ec143f1659a33.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/116fa9161cc3534a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/119ca9a8eb496ced.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/11a79a176b1d37b0.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/11c6ee172d78f042.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1222e8f00154e53e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/12380182bad5a7fb.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/123a4823e01ef69d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1267542c155bca73.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/127846b01a626672.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/12bddc46ec90c810.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/12d8ea83ccada998.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/12f086c96c9ee726.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/12fc4e07442b7f7a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1310f94581a6e22a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/132183327d61b086.md

配置与示例片段类

https://github.com/vhjhbkhggk/mqsaql/blob/main/134f30b70cd423cd.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1359e52054ca493f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/13975a23f72762d6.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/13ac7991dbe8d928.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/13faff8b53af5f6d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/140798584d9fa0c5.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1425a1cf454d31f2.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/14499e62abcfe6f3.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/146b6b075aea236d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1475333666fb409a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1499f42bce89b2f8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/14ae41af637bc117.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/14b62fef4d578f97.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/14c828223240ab06.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1525c7ef57cc1ab9.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/153c149d951f2b2a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/153d34f9330774c4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/155b823a3b510459.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/164ccb6f635156ef.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/16501d62dc1b5640.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/16701098607aaddd.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/168182f7ec88698e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1685b0fb9dc6b38d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1699d89f8eb3586f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/16c01ef361f1419c.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/16cfc441dc228fae.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/16e240d1e599fbc6.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/16f8b0c6992dab73.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/17036f55a61304e7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1706757b42584472.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/171efcebceccc7bd.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/173436e2044fe383.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/173f6c15b1704235.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1754bcea45039302.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/177a5f375e2195dc.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/179072e6924bc812.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/17aa176800569827.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/17aa5954ad966357.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/17b93b13b378b802.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/17c354b6febe1255.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1809c6429145f810.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/181238f050698b3d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1832e6521f251ddf.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1876b4495ab1c134.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/188396b73e73f3b9.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/18cbbece9ce40f77.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/18d0527ed1c6c495.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/18d5e4170e13008f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/18f2d1a6b7d7702e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/19174718f6813036.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/19347795897773dc.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/19351a7eef92a9e3.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/195911155a1d1cc9.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/195a2b3c44e5042d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/197bd171f37feabd.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/199bab651631cbde.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/19ded63802b1ca9b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/19e635b6aff5173b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/19f4fffa7d33c1c4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/19f62269161b48a7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/19fada1e84cfa745.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1a2997f1a7d509ec.md

运维与部署参考类

https://github.com/vhjhbkhggk/mqsaql/blob/main/1a362371f2e64ba8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1a5cf5c564428aab.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1a87d0d7cc71c2df.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1a8aa12052e99e59.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1a8faf7edf8c888a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1ab1d0d57dced9e8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1ab25b09ed2444ee.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1b0179f19876f5a8.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1b17b2d0a030703e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1b31cfd6de5f2b0a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1b4916e48b5ae6ad.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1b4a58e47afa3200.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1b7d64e8a21ea0e2.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1b86f270b2ec17b7.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1c0008dbab9410f4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1c049f6254def6e1.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1c40b6cb03586a3f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1c9933d151cd7c5f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1cb8e318f4e13b52.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1cbed337855f053d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1ccb8ba58f47357b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1ce726c777f571a6.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1d25e082479af534.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1d39de9f47ad58e9.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1d6dd03b95d3417e.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1d7c4750a6195040.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1d9a8b1889a1b833.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1db0bb63d1cc305a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1e2d024b189721fa.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1e3e8c24245f9e19.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1e4fb319ff0ba424.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1e83b17e753b98cf.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1e8512f87100b110.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1ebab9e7fdd2ca99.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1f0e5ceed65f2b4f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1f131e82b7b69fff.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1f27ba54af587e05.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1f586b2cecc271f3.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1f887d66969fdb01.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1fa46f5d30493ad4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1fccb36cff094d20.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/1fd74c41af5c19de.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/203534e92e45f6cd.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/205bc22eb210277b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/20752e6e85f23a21.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/20921a27c668a6b4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/20b9b82f91ff3418.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/20bb2c0c27389603.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/20cbb511e581c324.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/211598eb5dde4a10.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/211f2c9b441dedef.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/2168a0790dcedfc5.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/217fb71af9e1d797.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/21a63c25b4404aea.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/21bef5db7071492a.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/221334345b42a0b6.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/22193cfc321c24d4.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/221a72dc046e9faf.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/22322e5eb2f53adb.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/224013c0ead51e10.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/22650d0adbe31384.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/2282efa6576dd05d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/229f191da243bc2b.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/22ba9d83193fdeac.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/22c5ecc51c75fb8d.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/22c90d92093b8f0f.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/22cc6c95bcf869ac.md
https://github.com/vhjhbkhggk/mqsaql/blob/main/22e3b6feb81b5879.md

## 项目结构

```
linkvault/
├── README.md                         # 项目总览与使用入口
├── CONTRIBUTING.md                   # 贡献者操作流程与规范
├── CHANGELOG.md                      # 版本历史与批次变更记录
├── LICENSE                           # MIT 许可证全文
├── docs/                             # 文档目录
│   ├── resource_list.md              # 全量链接清单（按批次分类）
│   ├── batch_77.md                   # 第 77 批详细索引（当前批次）
│   └── batch_114.md                  # 第 114 批详细索引（待合并批次）
├── scripts/                          # 工具脚本目录
│   ├── build_index.sh                # 生成汇总索引的 Shell 脚本
│   ├── check_links.py                # 批量检查链接可达性的 Python 脚本
│   └── format_validator.sh           # 校验新增链接格式的 CI 辅助脚本
├── templates/                        # 模板文件
│   ├── new_batch_template.md         # 新批次链接的提交模板
│   └── category_header.md            # 分类标题的标准格式
├── archive/                          # 历史归档
│   └── batch_1_76/                   # 第 1 至 76 批历史快照
└── .github/                          # GitHub 自动化配置
    └── workflows/
        └── link_check.yml            # 每日定时执行链接检查的 GitHub Actions 工作流
```

## 贡献指南

1. 克隆项目仓库并在本地创建新的功能分支，分支命名格式为 `batch/xxx`，其中 xxx 为新增批次编号。确保分支基于最新的 main 分支创建。

2. 在 `docs/resource_list.md` 中追加新批次链接，严格遵循原有格式：每条链接独立成行，不添加额外前缀或后缀。若新增分类，需同步更新目录索引。

3. 运行本地检查脚本 `./scripts/format_validator.sh` 验证新增链接的格式合规性，并执行 `markdown-link-check docs/resource_list.md` 确认无失效链接。

4. 提交变更并推送到远程分支，随后在 GitHub 上发起 Pull Request。PR 描述中需注明批次编号、链接总数以及是否有分类调整。

5. 等待维护者审核。审核通过后由维护者合并至 main 分支，并同步更新 CHANGELOG.md 中的版本记录。

## 常见问题

Q: 为什么所有链接都指向同一个仓库的 blob 路径？

A: 本项目定位为外链汇总站，所有资源均来自用户提供的原始数据。这些链接指向的仓库作为上游来源，本项目不复制内容，仅提供结构化索引。如需查看具体内容，请直接访问对应链接。

Q: 如何确认某个链接是否仍然有效？

A: 项目通过 GitHub Actions 每日自动运行链接检查工作流，结果会输出到仓库的 Actions 页面。用户也可手动运行 `markdown-link-check docs/resource_list.md` 进行本地检查。

Q: 我可以提交非 GitHub 域名的外部链接吗？

A: 可以。但需确保链接是稳定、公开且与技术主题相关的资源。提交时请在 Pull Request 中说明链接用途及分类建议，便于审核。

## 许可证

MIT

> 外链数量: 180 | 生成时间: 2026-06-24 18:31:58
