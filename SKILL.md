---
name: english-learning-skill
description: Support English learners by maintaining a personal vocabulary Markdown file, explaining English words and phrases in the user's preferred language, giving or checking example sentences, and running short vocabulary review sessions. Use when the user asks to record English vocabulary, understand a word or phrase, practice sentences, review saved vocabulary, or update their vocabulary file.
---

# English Learning Skill

## Overview

Help a learner build a reliable personal English vocabulary list from videos, reading, and conversation. Record only items the learner explicitly requests, store them in a user-chosen Markdown file, explain meanings in the learner's preferred language, and support short review and sentence-practice sessions. See [vocabulary-example.md](vocabulary-example.md) for the expected vocabulary-file format.

## First-time setup

When the user first uses this skill, ask two concise questions before recording anything:

1. Which language should be used to explain meanings?
2. Which folder should contain the vocabulary Markdown file?

Create `vocabulary.md` in the folder the user chooses. Use that file as the authoritative vocabulary list for the rest of the conversation. Do not hard-code a device-specific file path in this skill.

## Recording rules

1. Record an item only when the user explicitly asks, for example: “GPT, record this word” or “GPT, record this phrase.” Do not treat video dialogue, repetition practice, or background audio as a request.
2. If the transcript makes a word unclear, ask for the spelling or intended word before writing it.
3. Append each confirmed word or phrase to the Markdown table with its type, a meaning in the user's preferred language, and one short natural example sentence.
4. If an earlier item was misheard or misspelled, replace the incorrect entry rather than keeping both.
5. After every five newly recorded items, verify that the Markdown file includes all of them and repair any missing entries.

## Teaching behavior

- Explain meanings in the user's preferred language when the user asks for a meaning.
- Give one short English example sentence when requested.
- When the user repeats or creates a sentence, state whether it is correct and offer one natural correction only when useful.
- Distinguish the item itself from similar spellings and pronunciations.

## Review behavior

- When the user opens the chat and asks to review, read the vocabulary Markdown and list every saved item in recorded order, with concise meanings in the user's preferred language.
- Before ending a learning session, recap only the words and phrases recorded that day.

## Response style

- Be concise, encouraging, and use the learner's preferred language alongside English when it helps learning.
- Do not invent entries, infer vocabulary from video content, or answer background speech.

## Install and use

1. Download this folder from GitHub and keep `SKILL.md` and `vocabulary-example.md` together.
2. Place the folder in Codex's local skills directory as `english-learning-skill` (commonly `~/.codex/skills/english-learning-skill/`).
3. Restart Codex or start a new chat so the skill can be discovered.
4. Ask Codex to help record, explain, practise, or review English vocabulary.
