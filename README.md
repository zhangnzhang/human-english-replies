# human-english-replies

English | [简体中文](README.zh-CN.md)

An AI skill that turns what you want to say — written in Chinese, any other language, or rough notes — into natural American English that sounds like a real person typed it. Built for small online sellers who answer customers, reviews and creators in English every day.

Works with Claude (as a Skill) and any agent that can read a Markdown instruction file.

## The problem

Machine-translated or AI-written replies are easy to spot: "I sincerely apologize for the inconvenience. Please don't hesitate to contact us." Customers read it as a template, and it quietly costs you trust, repeat orders and creator deals.

## What it does

- **Mirrors the other person.** Casual lowercase DM? Casual reply. Formal email? Slightly more formal — still human.
- **Writes with human rhythm.** Mixed sentence lengths, short fragments, contractions, one em dash at most.
- **Avoids AI-speak.** A built-in ban list of customer-service clichés, "AI vocabulary" and giveaway sentence patterns, each with a natural replacement.
- **Fits the situation.** Shipping updates, damage complaints, refunds, bad reviews, social comments, gift questions, creator outreach, and saying no politely.
- **Doesn't invent facts.** Order numbers, links, dates and policies come only from you; anything missing becomes a `[placeholder]`.
- **Speaks your niche (optional).** Fill in `niche-glossary-template.md` and it will use insider terms with enthusiasts — and avoid them with casual buyers.

See [example replies](examples/replies.md).

## Install

**Claude:** copy `skills/human-english-replies/` into `~/.claude/skills/` (or your project's `.claude/skills/`). Then paste the customer's message and what you want to say:

> Customer: "hey where's my order? i ordered like a week ago"
> 告诉他已经发货了，单号 #1234，大概 3 天到

**Other agents:** use `skills/human-english-replies/SKILL.md` as the instructions.

## Files

```
skills/human-english-replies/
├── SKILL.md                              # Voice, rhythm, mirroring, ban lists, workflow
└── references/
    └── niche-glossary-template.md        # Optional: your category's insider terms
examples/
└── replies.md                            # Before/after examples (fictional)
```

## License

[MIT](LICENSE)
