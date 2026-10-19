# human-english-replies

[English](README.md) | 简体中文

一个 AI Skill：你用中文（或其他语言、或零散的英文要点）说想表达什么，它帮你写成像真人打字的地道美式英文。专门给每天要用英文回复客户、评论和红人的跨境卖家。

可以作为 Claude 的 Skill 使用，也可以给任何能读 Markdown 指令文件的 AI 工具用。

## 解决什么问题

机翻或 AI 写的回复一眼就能看出来，比如「I sincerely apologize for the inconvenience. Please don't hesitate to contact us.」客户一看就知道是模板，信任、复购和红人合作都会悄悄受影响。

## 它能做什么

- **镜像对方语气。** 对方用全小写随手发消息，就随意地回；对方写正式邮件，就稍微正式一点，但依然像人。
- **写出真人的节奏。** 句子长短交错，有短句、有缩写，破折号一条最多一个。
- **避开 AI 腔。** 内置禁用清单，包括客服套话、典型 AI 词汇和一看就是 AI 的句式，每条都配了自然说法。
- **分场景回复。** 物流查询、损坏投诉、退款、差评、社媒评论、送礼咨询、红人邀约，还有怎么礼貌地拒绝。
- **不编造事实。** 订单号、链接、日期、政策只用你给的信息，缺了就留 `[占位符]` 提醒你补。
- **会说圈内话（可选）。** 填好 `niche-glossary-template.md`，它会对资深玩家用行话，对普通买家和送礼的人说大白话。

示例见[回复示例](examples/replies.md)。

## 安装

**Claude：** 把 `skills/human-english-replies/` 复制到 `~/.claude/skills/`（或项目里的 `.claude/skills/`），然后贴上客户消息和你想说的话：

> Customer: "hey where's my order? i ordered like a week ago"
> 告诉他已经发货了，单号 #1234，大概 3 天到

**其他 AI 工具：** 把 `skills/human-english-replies/SKILL.md` 作为指令文件。

## 文件结构

```
skills/human-english-replies/
├── SKILL.md                              # 人设、节奏、镜像法则、禁用清单、工作流程
└── references/
    └── niche-glossary-template.md        # 可选：填入你所在品类的圈内术语
examples/
└── replies.md                            # 回复前后对照示例（虚构）
```

## 许可证

[MIT](LICENSE)
