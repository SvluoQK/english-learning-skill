# English Learning Skill

这是一个用于英语学习的 Codex Skill，适合在看视频、读文章、聊天或练习口语时记录英语单词和短语。它会把你明确要求记录的词汇保存到 Markdown 文件中，并提供中文释义、词性、英文例句和复习支持。

## 安装

把仓库克隆到 Codex 的本地 skills 目录：

```bash
git clone https://github.com/SvluoQK/english-learning-skill.git ~/.codex/skills/english-learning-skill
```

然后重启 Codex，或开启一个新的 Codex 会话。

## 使用例子

第一次使用时，可以这样说：

```text
请使用 english-learning-skill 帮我记录英语词汇。
释义用中文，词汇文件放在 ~/Documents/English/vocabulary.md。
```

之后在学习过程中，可以直接让 Codex 记录、解释或复习：

```text
记录这个词：asylum
```

Codex 会解释含义，并把它写入你的词汇文件。

更推荐的方式是配合 Codex 的语音能力使用：看到或听到一个新单词时，直接用说话的方式告诉 Codex 你要记录这个单词。

例如你可以直接说：

```text
Codex，帮我记录这个单词：ominous。
```

也可以让它检查例句：

```text
我造句：Refugees are seeking asylum. 这句话自然吗？
```

或开始复习：

```text
帮我复习今天记录的单词。
```

## 效果示例

词汇文件会类似这样：

```markdown
# Vocabulary

| Word or phrase | Type | Meaning | Example |
| --- | --- | --- | --- |
| asylum | noun | 庇护；避难所 | Refugees are seeking asylum. |
| infringe on | verb phrase | 侵犯；违背（权利等） | This rule may infringe on our rights. |
| ominous | adjective | 不祥的；预示坏事的 | The ominous silence made her nervous. |

## Daily recap

### 2026-08-14

- asylum
- infringe on
- ominous
```

## 适合场景

- 看英文视频时，随手记录听到的新词。
- 阅读英文文章时，保存高频词和短语。
- 练习口语或写作时，让 Codex 检查例句是否自然。
- 每天结束学习前，复习当天记录的词汇。
