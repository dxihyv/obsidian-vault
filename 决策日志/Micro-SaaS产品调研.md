# Micro SaaS 产品调研报告

> 数据来源：训练数据 + GitHub API + 有限网络抓取
> 更新：2026-05-02

---

## 一、已验证的独立开发者案例（含营收）

| 产品 | 创始人 | 赛道 | 营收 | 特点 |
|------|--------|------|------|------|
| Nomad List | Pieter Levels | 远程工作者社区 | $80K+/月 | 全自动、零员工 |
| Remote OK | Pieter Levels | 远程工作招聘 | 同上（打包） | 蹭Nomad流量 |
| Buffer | Joel Gascoigne | 社交媒体排程 | $18M+/年 | 融资但早期bootstrapped |
| EmailOctopus | Marc Lou | 邮件营销替代SendGrid | $2M+/年 | AWS SES中间层，便宜80% |
| Carrd | Josh Anderson | 简单着陆页 | $2M+/年 | 极简、$19/年/站 |
| Plausible | Marko Saric/Uku Täht | Google Analytics替代 | $1M+/年 | 隐私优先、便宜90% |
| IndieHackers.com | Courtland Allen | 独立开发者社区 | 卖掉 | 被Stripe收购 |
| Instapainting | — | 照片转油画 | $32K/月 | 图片处理+手工 |
| Tim博客辅助工具 | Tim | 内容工具 | $2.5K/月 | 博客+工具组合 |
| 3个SaaS工具组合 | 不知名 | 多工具 | $400K+/年 | 多产品组合 |

### 华人/出海案例
| 产品 | 创始人 | 赛道 | 营收 |
|------|--------|------|------|
| uTools | — | 效率工具平台 | 插件生态盈利 |
| 稿定设计 | — | 在线设计 | 融资规模化 |
| 即刻工具 | — | 小程序/效率 | 社群驱动 |

---

## 二、成功的4种模式

### 1. 替代昂贵方案 → 便宜80-90%
- EmailOctopus：替代SendGrid，价格低80%，用AWS SES
- Plausible：替代Google Analytics，价格低90%
- Carrd：替代Squarespace/Wix，$19/年 vs $100+/月

**龙哥启示：** 先问"什么工具大家觉得贵？" → 建一个便宜版本

### 2. 垂直 niche → 没有人做的小赛道
- Nomad List：只做远程工作者社区，大厂不屑于做
- Instapainting：只做照片转油画，全世界就这一个

**龙哥启示：** "这个细分需求有没有现成工具？" 比 "这个市场有多大" 更重要

### 3. 自动化重复操作
- Buffer：替代每天手动发社交媒体
- 各种Zapier/Make类工具

**龙哥启示：** "我每天重复什么事情？" → 自动化

### 4. 内容/社区 + 工具组合
- Tim：博客写内容 → 工具变现
- Indie Hackers：社区 + 工具

**龙哥启示：** 先用内容建立信任，再卖工具

---

## 三、找到痛点的调研路径

### 最有效（龙哥优先用这个）
1. **Twitter/X 搜索**："I'm building..." "Launched my..." "Made $X with..."
2. **Indie Hackers Forum**：真实收入分享区
3. **Product Hunt 新品**：看人们在解决什么问题

### 次选
4. **GitHub Trending**：看什么工具被疯狂star
5. **逆向收费产品**：在Stripe Atlas、Gumroad看什么卖得好

### 社区资源（Indie Hacker Wiki）
- 顶级博客：levels.io, jakobgreenfeld.com, marketingexamples.com, tinylittlebusinesses.com
- 播客：Indie Bites, Ramen FM, Bootstrapped
- 社区：WIP.co, Ramen Club, Product Hunt, Hacker News

---

## 四、工具链（从 indie-hacker-tools 整理）

### 开发栈
- **前端**：Next.js 15 + v0.dev (AI生成UI)
- **部署**：Vercel / Zeabur / Cloudflare Workers
- **数据库**：Supabase / Cloudflare R2 / Planetscale
- **认证**：Auth.js / Better Auth
- **支付**：Stripe / Creem（专为独立开发者设计）

### 增长/SEO
- **SEO工具**：Ahrefs, AITDK（免费AI SEO）
- **爬虫/数据**：Firecrawl（网站转LLM数据）
- **邮件**：Resend

### 无代码/MVP快速验证
- **模板**：Nextjs SaaS Template（GitHub有）
- **自动化**：n8n（自托管工作流）

---

## 五、龙哥的行动建议

### 这周可以做的事（2小时）
1. 列出每天重复做的3件事（哪怕很小：比如"每天要把同一张图发到3个平台"）
2. 其中1件问："有没有更简单的方式？" 如果没有 → 机会
3. 用 uTools + 现有AI工具快速验证

### 下一步（如果有眉目）
1. 用 [六个问题检查清单](/cos/obsidian/决策日志/新项目启动检查.md) 评估
2. 目标：找到一个"每天浪费30分钟"的操作 → 自动化
3. 先做MVP验证，再考虑做大

---

## 六、参考资料

- awesome-indiehackers (johackim) - Indie Hacker资源大全
- indie-hacker-tools (tmstack) - 独立开发者工具导航
- 关键博客：levels.io, jakobgreenfeld.com, marketingexamples.com
- 播客：Indie Bites, Ramen FM
