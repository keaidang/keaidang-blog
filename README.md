# keaidang.com · 个人博客

部署在腾讯云 **EdgeOne Pages**，主域名 keaidang.com 作为博客首页。

## 当前状态

🚧 **部署测试阶段** — 当前为静态测试页（无构建），用于验证 EdgeOne Pages 的部署链路、域名解析和 HTTPS 证书。

## 部署信息（EdgeOne Pages 配置参考）

| 配置项 | 值 |
|---|---|
| 仓库 | `github.com/keaidang/keaidang-blog` |
| 分支 | `main` |
| 构建命令 | （留空，静态页面） |
| 输出目录 | `./`（仓库根目录） |
| 自定义域名 | keaidang.com |

DNS 解析（域名服务商处添加，不影响已有邮件 MX 记录）：

```
类型   主机记录   记录值
CNAME  @        <EdgeOne 分配的接入地址>
```

> ⚠️ 注意：只新增解析记录，不要删除/修改已有的 MX、SPF、DKIM 记录，@keaidang.com 邮箱服务依赖它们。

## Roadmap

- [ ] EdgeOne Pages 部署测试（当前）
- [ ] 域名解析 + HTTPS 验证
- [ ] 迁移到 **Astro** 博客框架（文章 Markdown 化、主题定制）
- [ ] 评论系统（giscus，基于 GitHub Discussions）
- [ ] 柯南分享站迁移至 conan.keaidang.com

## 相关仓库

- [keaidang/conan-site](https://github.com/keaidang/conan-site) — 名侦探柯南动漫分享站

---

© 2026 keaidang.com
