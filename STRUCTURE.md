# 牛马生涯 — 项目目录结构设计

## 设计理念

按照内容的**性质**和**用途**分层组织，让读者可以按需阅读：
- 想系统学习 → 看「主题指南」
- 想看真实故事 → 看「案例故事」
- 想看分享回放 → 看「演讲分享」
- 想要工具模板 → 看「资源工具箱」

---

## 目录结构

```
NiuMaCareer/
│
├── README.md                        # 项目介绍与导航
├── STRUCTURE.md                     # 本文件：目录结构说明
├── CHANGELOG.md                     # 更新日志
│
├── topics/                          # 📚 主题指南（系统性内容）
│   ├── README.md                    # 主题索引与阅读指南
│   ├── 01-job-hunting/              # 求职篇
│   │   ├── resume.md                # 简历怎么写
│   │   ├── interview.md             # 面试心法
│   │   ├── offer-decision.md        # 如何选 offer
│   │   └── salary-negotiation.md    # 谈薪策略
│   ├── 02-workplace/                # 职场篇
│   │   ├── first-year.md            # 第一年存活指南
│   │   ├── communication.md         # 职场沟通
│   │   ├── manage-up.md             # 向上管理
│   │   └── collaboration.md         # 跨团队协作
│   ├── 03-growth/                   # 成长篇
│   │   ├── career-stages.md         # 1-5-10 年阶段论
│   │   ├── depth-vs-breadth.md      # 深度 vs 广度
│   │   ├── job-hopping.md           # 跳槽时机与策略
│   │   └── tech-to-management.md    # 技术转管理
│   ├── 04-mindset/                  # 心态篇
│   │   ├── anxiety.md               # 焦虑与内卷
│   │   ├── meaning.md               # 工作的意义感
│   │   └── survival-life-purpose.md # 生存-生活-生命框架
│   └── 05-ai-era/                   # AI 时代篇
│       ├── ai-career-impact.md      # AI 对职业的冲击
│       ├── ai-enhanced-work.md      # 用 AI 提效的实操
│       └── future-proof.md          # 如何不被淘汰
│
├── cases/                           # 📖 案例故事（场景化内容）
│   ├── README.md                    # 案例索引
│   ├── interview/                   # 面试相关案例
│   │   ├── case-001-first-offer.md  # 我的第一个 offer
│   │   └── case-002-failed-xxx.md   # 挂在 xxx 的那次面试
│   ├── workplace/                   # 职场场景案例
│   │   ├── case-001-conflict.md     # 和同事产生分歧
│   │   └── case-002-promotion.md    # 第一次晋升
│   ├── decision/                    # 关键选择案例
│   │   ├── case-001-startup-or-big.md   # 大厂 vs 创业公司
│   │   └── case-002-stay-or-leave.md    # 该不该跳槽
│   └── ai-practice/                 # AI 实践案例
│       ├── case-001-ai-coding.md    # 用 AI 写代码的真实体验
│       └── case-002-ai-interview.md # AI 时代面试的变化
│
├── presentations/                   # 🎤 演讲分享（线下/线上分享记录）
│   ├── README.md                    # 分享列表索引
│   └── 01-AI时代下的少年/
│       ├── README.md                # 分享概要
│       ├── script.md                # 详细脚本/逐字稿
│       ├── slides/                  # 演示材料
│       └── feedback.md              # 分享后反馈与复盘
│
├── resources/                       # 🧰 资源工具箱
│   ├── README.md                    # 资源索引
│   ├── templates/                   # 模板
│   │   ├── resume-template.md       # 简历模板
│   │   └── self-intro-template.md   # 自我介绍模板
│   ├── reading-list.md              # 推荐书单/文章
│   ├── tools.md                     # 好用的工具推荐
│   └── links.md                     # 外部优质资源链接
│
└── .github/                         # GitHub 配置
    └── ISSUE_TEMPLATE/
        └── question.md              # 读者提问模板
```

---

## 命名规范

| 维度 | 规范 | 示例 |
|------|------|------|
| 主题目录 | `数字序号-英文关键词/` | `01-job-hunting/` |
| 主题文章 | `英文短横线命名.md` | `offer-decision.md` |
| 案例文件 | `case-序号-关键词.md` | `case-001-first-offer.md` |
| 分享目录 | `序号-中文主题/` | `01-AI时代下的少年/` |

---

## 内容定位区分

| 类型 | 定位 | 特点 | 适合场景 |
|------|------|------|---------|
| 主题指南 `topics/` | 系统化知识 | 结构化、有框架、可反复查阅 | 想系统了解某个方向 |
| 案例故事 `cases/` | 真实场景 | 故事性、有细节、有情绪 | 想看别人怎么做的 |
| 演讲分享 `presentations/` | 现场记录 | 有时间线、有互动、有反馈 | 想了解分享现场 |
| 资源工具 `resources/` | 实用工具 | 可直接拿走用 | 想要模板或推荐 |

---

## 交叉引用建议

内容之间可以互相引用，形成网络：
- 主题文章中引用相关案例：`> 相关案例：[我的第一个 offer](../cases/interview/case-001-first-offer.md)`
- 案例中引用主题框架：`> 这属于"生存阶段"的典型问题，详见 [生存-生活-生命框架](../topics/04-mindset/survival-life-purpose.md)`
- 分享脚本中引用主题和案例作为素材来源
