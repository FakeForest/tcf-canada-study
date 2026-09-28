# TCF Canada French Project Instructions

## Purpose

This folder stores the user's French-learning materials and study notes for TCF Canada. The user makes French notes from their PC and may continue the work across devices through Obsidian Sync. Files updated or added from the MacBook and from the PC are expected to sync into this same folder. When extracting, editing, or reorganizing source material, preserve the user's own handwritten learning system.

## Project Boundary

- The Obsidian vault is `Jason's Knowledge Vault`.
- The French project lives inside the `TCF Canada French` folder.
- Only read or edit files inside `TCF Canada French` unless the user explicitly asks for work somewhere else.
- The vault may contain unrelated folders, such as ECE graduate-study notes. Do not mix French materials with those folders.
- Preserve original source PDFs, PowerPoints, textbooks, exercise books, and user-created notes.

## AGENTS.md Handling Rule

- There should be only one `AGENTS.md` inside `TCF Canada French`.
- If `TCF Canada French/AGENTS.md` already exists through Obsidian Sync, update that same file.
- Do not create another `AGENTS.md`, `Agent.md`, `agent.md`, or duplicate instruction file.
- If `TCF Canada French/AGENTS.md` does not exist, create it from `French Notes Agent Handoff.md`.
- Keep `French Notes Agent Handoff.md` as the portable cross-device guide, and keep `AGENTS.md` as the active local instruction file for Codex.

## Current Folder Structure

- `Pronunciation and Numbers`: notes extracted from the user's French pronunciation PDF and number/pronunciation materials.
- `French Textbook/A1`: completed A1 Lessons 01-36, original textbook/supplement PDFs, and Assets. Moved together on 2026-09-28 at the user's request; preserve original filenames and contents.
- `French Textbook/A2`: A2 textbook, supplemental PDFs, and new A2 lesson notes. Lesson numbering restarts at 01.
- `Textbook Exercises`: exercise-book files or future extracted exercise notes.
- `Vocabulary`: future vocabulary notes, including gender, plural forms, and useful forms.
- `tmp`: temporary extraction/rendering files if present. Do not treat it as study content.

## Language Rules

- French is the main study content.
- English and Chinese support understanding.
- Notes may contain French, English, and Chinese, but do not force every item to be trilingual.
- Add English or Chinese only when it is present in the source, useful for understanding, or requested by the user.
- For textbook lesson notes, visible section titles, review prompts, and grammar explanations should be Chinese-first so the user can review more smoothly.
- Bracketed English, such as `[book]`, means English meaning/translation.
- Unbracketed English-like or romanized writing is usually the user's pronunciation cue, not an English meaning.
- Handwritten Chinese may be a Chinese meaning, grammar note, pronunciation explanation, or other study note. Preserve its role based on context.

## Handwritten Annotation Conventions

- A crossed-out or slashed French letter means the letter is silent / 不发音.
- If the final `t` in **salut** is crossed out, write that the final `t` is not pronounced.
- Handwritten arrows, substitutions, and syllable-like spellings describe how the user hears or remembers pronunciation.
- Preserve personal learner cues beside the relevant French text instead of replacing everything with standard IPA.
- Use standard IPA only when it is printed clearly in the source.
- If handwriting is unclear, mark it with `(?)` or place it in an `Items to Confirm` callout. Do not invent an answer.

## Pronunciation Cue Placement

Place handwritten pronunciation cues directly beside the French word or phrase they explain.

Preferred:

```markdown
**Excusez-moi** (`ex + gyu + z + ei + mua`) - excuse me
```

Avoid collecting clear word-level cues only in a separate list when they can be attached beside the original phrase.

## Extraction Rules

- Base notes strictly on the supplied PDF, PowerPoint, textbook, exercise book, or user annotation.
- Preserve the difference between printed source content, handwritten annotations, translations, and pronunciation cues.
- Do not invent missing meanings, grammar rules, pronunciation rules, or corrections.
- Keep notes useful for review, not just exhaustive transcription.
- When the user asks to extract from a textbook lesson, avoid practice/exercise pages unless explicitly requested.
- For textbook lesson notes, prefer this review structure: `课文 + 单词 + 语法`.

## Obsidian Formatting Style

- Use the `balanced-study-note` CSS class for extracted French study notes.
- Prefer clear headings, Obsidian callouts, compact tables, and page-level PDF links.
- Keep Markdown readable even without custom CSS.
- Link each extracted section to the original PDF page with Obsidian wikilinks when possible.

PDF 页面链接示例:

```markdown
> 来源: [[taxi_1学生用书9.23.pdf#page=30|查看教材 PDF - 第 30 页]]
```

## Textbook Note Style

- Textbook lesson files should be named with a zero-padded lesson number so Obsidian sorts them correctly.
- Filename example: `Lesson 01 - Bienvenue.md`.
- Visible title example: `# Lesson 1 - Bienvenue !`.
- Include source/frontmatter when useful:

```markdown
---
cssclasses:
  - balanced-study-note
source: "[[taxi_1学生用书9.23.pdf]]"
lesson: 1
pages: 26-28
---
```

Preferred lesson structure:

```markdown
# Lesson 1 - Bienvenue !

> [!info] 如何阅读这些笔记
> - 法语是主要学习内容。
> - `[English]` 或破折号后的英文可作为含义提示。
> - 法语旁边的英语式拼读通常是发音/记忆提示。
> - 中文用于解释意思、语法或来源批注。

## 课文

## 单词

## 语法

## 快速复习
```

## Textbook Extraction Boundary

- Do not extract practice/exercise sections unless the user explicitly asks.
- The user's current textbook-note goal is review: easy to see, easy to remember, easy to come back to.
- The user will continue updating the textbook PDF after each new French class (`每上一节新的法语课`). Before extracting a new lesson, read the latest synced textbook PDF and its newest annotations instead of assuming the PDF is unchanged.
- The user may replace the textbook PDF with a newer annotated version (`最新有笔记的版本`). When that happens, check existing lesson-note PDF wikilinks and update them so each note points to the current textbook PDF and correct page target.
- After every textbook PDF update, scan every `French Textbook/<affected level>/Lesson *.md` file, including frontmatter, page-level links, and the final source line. Replace older filenames only for that same textbook/level. Preserve page targets when pagination is unchanged; otherwise verify and update them. Verify zero obsolete links remain within the affected level before reporting completion.
- For each lesson, focus on dialogues/texts, vocabulary, and grammar structures already learned.
- Handwritten cues should appear beside the specific French phrase or word when clear.

## Known Textbook Work Already Done

### A2 Current Work

- Current A2 textbook: `French Textbook/A2/你好法语2.pdf` (252 PDF pages).
- Current A2 supplement: `French Textbook/A2/你好法语A2第一单元.pdf` (15 pages).
- A2 Lesson 1 is `French Textbook/A2/Lesson 01 - Je me presente.md`: textbook PDF pages 12-15, with both dialogues translated sentence by sentence; page 14 exercises excluded.
- The user specifically requests that A2 Lesson 1 emphasize the Unit 1 slides: visible U1L1 content is on pages 2-5 (vocabulary, quel, three question forms, inversion). Page 6 begins U1L2; do not extract L2 or later until requested.
- Preserve A1's Chinese-first explanations, handwritten cues, review structure, CSS class, and page links for A2.
- Keep textbook-version tracking separate by level. A2 updates must NEVER replace A1 textbook links. Sweep all lesson notes within the affected level after each new PDF, verify pagination against that edition, and check zero obsolete links within that level.
- A1 links remain on `taxi_1学生用书9.23.pdf`; A2 links currently use `你好法语2.pdf`. Do not treat A2 as a newer edition of A1.
- Use level-qualified paths when a note name becomes ambiguous across A1/A2. Shared Vocabulary and Pronunciation folders remain unchanged.
- Only the project-root AGENTS.md is used; do not create per-level agent files.

### A1 Completed Work

The current A1 textbook PDF is `French Textbook/A1/taxi_1学生用书9.23.pdf`. Preserve earlier PDF versions if present; use this PDF for A1 lesson notes, not for A2.

The user has completed all 36 lessons. Notes are updated through Lesson 36 using `taxi_1学生用书9.23.pdf`. Lesson 33 starts at PDF page 176, Lesson 34 at page 180, Lesson 35 at page 184, and Lesson 36 at page 188; Lesson 36 is extracted through page 191. Later exercise/review pages are not additional lessons.

Lesson 1-36 `课文` sections use sentence-level French-Chinese review tables where practical, matching the Lesson 22-23 style.

Supplemental grammar sources currently copied into `French Textbook`:

- `French Textbook/A1/你好法语A1第一单元.pdf`: Unit 1 PDF export; grammar/vocabulary supplement for Lessons 1-4.
- `French Textbook/A1/你好法语A1第二单元.pdf`: Unit 2 PDF export; grammar/vocabulary supplement for Lessons 5-8.
- `French Textbook/A1/你好法语A1第三单元.pdf`: Unit 3 PDF export; grammar/vocabulary supplement for Lessons 9-12.
- `French Textbook/A1/你好法语A1第四单元.pdf`: Unit 4 PDF export; grammar/vocabulary supplement for Lessons 13-16.
- `French Textbook/A1/你好法语A1第五单元.pdf`: Unit 5 PDF export; grammar/vocabulary supplement for Lessons 17-20.
- `French Textbook/A1/你好法语A1第六单元.pdf`: Unit 6 PDF export; supplements for Lessons 21-24 (pages 2-16). Its final pages revisit earlier lessons; follow the actual L marker rather than the filename.
- `French Textbook/A1/你好法语A1第七单元.pdf`: Unit 7 PDF export; supplements for Lessons 25-27 (pages 2-15). No separate L28 material is present; Lesson 28 remains textbook-based.
- `French Textbook/A1/你好法语A1第八单元.pdf`: Unit 8 PDF export; supplements for Lessons 29-32 (pages 2-9).
- `French Textbook/A1/你好法语A1第九单元.pdf`: All 23 pages checked. Pages 2-13 supplement L33, pages 14-18 supplement L34, and pages 19-23 supplement L35. Page 1 is the cover; there is no separate L36 slide. Grammar, vocabulary, examples, and maps are integrated; listening prompts/empty tables are referenced without invented answers.
- `French Textbook/A1/Assets/passe-compose-etre-verbs.png`: cropped image from Unit 5 supplement for common `être` auxiliary verbs in the passé composé; embedded in Lesson 19.
- `French Textbook/A1/你好法语A1第一单元.pptx`: original Unit 1 PowerPoint source.
- `French Textbook/A1/你好法语A1第二单元.pptx`: original Unit 2 PowerPoint source.

When using these sources, the lesson number is shown by the `L` number in the upper-left lesson marker, such as `U1L2` or `U2L7`. Prefer linking lesson notes to the PDF exports because Obsidian previews PDFs more reliably than PPTX files.

Lesson notes already created previously:

- `French Textbook/A1/Lesson 01 - Bienvenue.md`
- `French Textbook/A1/Lesson 02 - Qui est-ce.md`
- `French Textbook/A1/Lesson 03 - Ca va bien.md`
- `French Textbook/A1/Lesson 04 - Correspondants.md`
- `French Textbook/A1/Lesson 05 - Trouvez l'objet.md`
- `French Textbook/A1/Lesson 06 - Portrait-robot.md`
- `French Textbook/A1/Lesson 07 - Shopping.md`
- `French Textbook/A1/Lesson 08 - Le coin des artistes.md`
- `French Textbook/A1/Lesson 09 - Appartement a louer.md`
- `French Textbook/A1/Lesson 10 - C'est par ou.md`
- `French Textbook/A1/Lesson 11 - Bon voyage.md`
- `French Textbook/A1/Lesson 12 - Marseille.md`
- `French Textbook/A1/Lesson 13 - Un aller simple.md`
- `French Textbook/A1/Lesson 14 - A Londres.md`
- `French Textbook/A1/Lesson 15 - Le dimanche matin.md`
- `French Textbook/A1/Lesson 16 - Une journee avec Laure Manaudou.md`
- `French Textbook/A1/Lesson 17 - On fait des crepes.md`
- `French Textbook/A1/Lesson 18 - Il est comment.md`
- `French Textbook/A1/Lesson 19 - Chere Lea.md`
- `French Textbook/A1/Lesson 20 - Les fetes.md`
- `French Textbook/A1/Lesson 21 - C'est interdit.md`
- `French Textbook/A1/Lesson 22 - Petites annonces.md`
- `French Textbook/A1/Lesson 23 - Qu'est-ce qu'on lui offre.md`
- `French Textbook/A1/Lesson 24 - Le candidat ideal.md`
- `French Textbook/A1/Lesson 25 - Enquete.md`
- `French Textbook/A1/Lesson 26 - Quitter Paris.md`
- `French Textbook/A1/Lesson 27 - Vivement les vacances.md`
- `French Textbook/A1/Lesson 28 - Les Francais en vacances.md`
- `French Textbook/A1/Lesson 29 - Enfant de la ville.md`
- `French Textbook/A1/Lesson 30 - Fait divers.md`
- `French Textbook/A1/Lesson 31 - Ma premiere histoire d'amour.md`
- `French Textbook/A1/Lesson 32 - La 2CV.md`
- `French Textbook/A1/Lesson 33 - Beau fixe.md`
- `French Textbook/A1/Lesson 34 - Projets d'avenir.md`
- `French Textbook/A1/Lesson 35 - Envie de changement.md`
- `French Textbook/A1/Lesson 36 - Le pain, mangez-en.md`

PPT grammar supplements already added:

- Lessons 1-4: supplemented from `你好法语A1第一单元.pdf`.
- Lessons 5-7: supplemented from `你好法语A1第二单元.pdf`.
- Lesson 8: Unit 2 supplemental source contains vocabulary/课文 material, but no major extra grammar supplement was added.
- Lessons 9-12: supplemented from `你好法语A1第三单元.pdf` where useful.
- Lessons 13-16: supplemented from `你好法语A1第四单元.pdf` where useful.
- Lessons 17-20: supplemented from `你好法语A1第五单元.pdf` where useful.
- Lesson 19: includes the cropped `être` auxiliary verb image from `你好法语A1第五单元.pdf`.
- Lessons 21-24: supplemented from Unit 6, including COI positions, futur proche, COD comparisons, second-group verbs, and interview vocabulary.
- Lessons 25-27: supplemented from Unit 7, including quantity/en, ça, tout, pronominal verbs, and past-participle agreement exceptions. Unit 7 has no dedicated Lesson 28 supplement.
- Lessons 29-32: supplemented from Unit 8, including imparfait forms/use, verb constructions, seasons/love expressions, fabriquer and présenter.
- Lessons 33-35: supplemented from Unit 9, including weather/directions, futur simple forms and spelling changes, en with de complements, certainty, future-time comparisons, telephone expressions, verb constructions, si/quand, changer/changer de, and renovation vocabulary. Lesson 33 embeds maps from slides 9-10 as `Assets/unit9-france-map.png` and `Assets/unit9-france-regional-words.png`. Lesson 36 records the complete Unit 9 coverage map and remains textbook-based.
- Some supplemental PDF text layers repeat hidden content from other slides. Verify visible page headings and actual page numbers before assigning source links. Source typos corrected in the notes are explicitly identified.

Page boundaries used before:

- Lesson 1: pages 26-28; exercise/practice page excluded.
- Lesson 2: pages 30-32; page 33 exercise/pronunciation excluded.
- Lesson 3: pages 34-36; page 37 exercise/pronunciation excluded.
- Lesson 4: pages 38-40; exercise/practice content excluded.
- Lesson 5: pages 44-46; page 47 exercise/pronunciation excluded.
- Lesson 6: pages 48-50; page 51 exercise/pronunciation excluded.
- Lesson 7: pages 53-55; page 56 exercise/pronunciation excluded.
- Lesson 8: pages 58-59; later cultural/exercise pages not extracted unless requested.
- Lesson 9: pages 64-66; page 67 exercise/pronunciation excluded.
- Lesson 10: pages 68-70; page 71 exercise/pronunciation excluded.
- Lesson 11: pages 72-74; page 75 exercise/pronunciation excluded.
- Lesson 12: pages 76-78; page 80 savoir-faire/practice page not extracted as a lesson note.
- Lesson 13: pages 84-86; page 87 exercise/pronunciation excluded.
- Lesson 14: pages 88-90; page 91 exercise/pronunciation excluded.
- Lesson 15: pages 92-94 extracted; page 95 exercise/pronunciation excluded.
- Lesson 16: pages 96-98 extracted; later practice/cultural review pages excluded unless requested.
- Lesson 17: pages 102-104 extracted; grammar on page 104 included, exercises not transcribed unless they support the grammar explanation.
- Lesson 18: pages 106-109 extracted; page 108 grammar included, page 109 communication/pronunciation used only for review expressions.
- Lesson 19: pages 110-113 extracted; page 112 grammar included, page 113 communication/pronunciation used only for review expressions.
- Lesson 20: pages 114-117 extracted; pages 116-117 culture/communication used only where helpful for review.
- Lesson 21: pages 120-123 extracted; page 122 grammar included, page 123 communication/pronunciation used only where helpful for review.
- Lesson 22: pages 124-127 extracted; page 126 grammar included, page 127 communication/pronunciation used only where helpful for review.
- Lesson 23: pages 128-131 extracted; page 130 grammar included, page 131 communication/pronunciation used only where helpful for review.
- Lesson 24: pages 132-135 extracted; page 134 communication/culture used only where helpful for review, page 135 Chinese summary and employment-culture note used as support.
- Lesson 25: pages 140-143 extracted; page 142 grammar included, page 143 communication/pronunciation used only where helpful for review.
- Lesson 26: pages 144-147 extracted; page 146 grammar included, page 147 communication/pronunciation used only where helpful for review.
- Lesson 27: pages 148-151 extracted; page 150 grammar included, page 151 communication/pronunciation used only where helpful for review.
- Lesson 28: pages 152-155 extracted; survey data and point-of-view text included, page 155 culture note used as support; page 156 Savoir-faire excluded.
- Lesson 29: pages 158-161 extracted; page 160 grammar included, page 161 communication/pronunciation used only where helpful for review.
- Lesson 30: pages 162-165 extracted; page 164 grammar included, page 165 communication/pronunciation used only where helpful for review.
- Lesson 31: pages 166-169 extracted; page 168 grammar included, page 169 pronunciation and Chinese text translation used only where helpful for review.
- Lesson 32: pages 170-173 extracted; sentence-level text from pages 170-171, handwritten vocabulary cues and textbook notes included. Page 172 symbol vocabulary and page 173 Chinese translation support review; exercise prompts are not transcribed.
- Lesson 33: pages 176-179; weather dialogue, vocabulary, handwritten cues, impersonal verbs, futur simple and certainty; exercise prompts excluded.
- Lesson 34: pages 180-183; telephone dialogue, future plans, vocabulary, handwritten cues, and three ways to express the future; exercise prompts excluded.
- Lesson 35: pages 184-187; apartment dialogue, renovation vocabulary, handwritten cues, si/quand and changer constructions; exercise prompts excluded.
- Lesson 36: pages 188-191; bread texts translated sentence by sentence, en/y order, ne...plus, neutral le, polite imparfait, and supporting geography vocabulary. Textbook statistics are explicitly historical source data, not current statistics; exercise prompts excluded.

## Pronunciation Notes Already Created

Source PDF: `Pronunciation and Numbers/法语语音笔记.pdf`.

Existing extracted notes:

- `Pronunciation and Numbers/00 French Pronunciation Course - Index.md`
- `Pronunciation and Numbers/01-05 Introduction and French Alphabet.md`
- `Pronunciation and Numbers/06-13 Pronunciation Foundations.md`
- `Pronunciation and Numbers/14-18 Numbers 0-10 and Core Sounds.md`
- `Pronunciation and Numbers/19-22 Numbers 11-29 and E Vowels.md`
- `Pronunciation and Numbers/23-27 Numbers 30-99 and K-S Sounds.md`
- `Pronunciation and Numbers/28-35 Age, Etre, and Rounded Vowels.md`
- `Pronunciation and Numbers/36-41 Nationalities and G-Z-NY Sounds.md`
- `Pronunciation and Numbers/42-45 Liaison, Elision, and Nasal Vowels.md`
- `Pronunciation and Numbers/46-56 Semivowels, X, and Final Reading.md`

These filenames use numeric page prefixes to preserve PDF order in Obsidian while keeping readable titles.

## Pronunciation Notes Style

- Keep printed rules in the language used by the PDF. If the PDF rule is Chinese, extract it in Chinese instead of translating it into English.
- Put page links under page content so the user can jump back to the original PDF.
- Preserve the user's cue system. Example: **Excusez-moi** should show a cue like `ex + gyu + z + ei + mua` if that is what the handwritten note indicates.
- If a handwritten cue is inferred from context, be conservative and mark uncertainty when needed.

## Vocabulary Folder Plan

Current filled verb conjugation PDF:

- `Vocabulary/不规则变位与过去分词 - 已填.pdf`: updated through Lesson 23; includes the core conjugation table plus a Lesson 22-23 supplement for `falloir` and regular second-group `-ir` verbs. It has not yet been refreshed for Lesson 24-36 unless the user asks.
- `Vocabulary/未完成过去时与简单将来时变位表 - 已填.pdf`: filled on 2026-09-08 with imparfait and futur simple forms for the 24 verbs in the source table.

Future vocabulary notes should record:

- French word or phrase.
- English/Chinese meaning when useful or present in source.
- Gender for nouns: `m.` or `f.`.
- Plural form when relevant.
- Useful verb forms or adjective forms when relevant.
- Example sentence if it helps review.
- Source lesson or PDF page when available.

## Safety Rules

## GitHub Backup After Note Updates

- The user requests a new repository named `tcf-canada-study` for this entire French project and a commit/push after every future French-note update.
- The user explicitly requested public visibility after initial setup. This repository is public; notes, source materials, annotations, and committed history are accessible to anyone. Never commit credentials or unrelated private data.
- Include all study notes, original source PDFs/PPTX, images, Vocabulary, Textbook Exercises, and both project instruction documents. Exclude only temporary extraction output (`tmp/`), operating-system caches, credentials, and Git internals.
- Repository: `https://github.com/FakeForest/tcf-canada-study` (public, at the user's explicit request), remote `origin`, branch `main`. GitHub CLI is authenticated as `FakeForest` and Git uses its credential helper. Always verify the remote commit after each push; local commits alone are not a completed backup.
- Official tools are installed at `~/.local/bin/gh` and `~/.local/bin/git-lfs`; include `~/.local/bin` in PATH for Git operations. Git LFS is configured locally and PDF/PPTX sources are tracked with LFS.
- Configure Git LFS for large source PDFs before the initial commit; never silently omit a large source file. Explain any storage quota or billing requirement before proceeding.
- After each requested note update: validate notes and links, inspect all project changes for secrets/unrelated content, stage intended French study changes, commit with a concise descriptive message, push to the verified remote, and verify the remote commit matches the local commit.
- Do not force-push, discard user edits, or automatically resolve cross-device conflicts. Report authentication, network, quota, or conflict blockers accurately.
- This rule applies when an agent performs note work. It does not by itself install a background watcher or automatically upload edits made on another device. Do not claim continuous sync is active.
- Keep Obsidian Sync as the cross-device note workflow; do not move this repository boundary outside `TCF Canada French`.

## File Safety

- Do not delete, rename, or broadly reorganize notes unless the user explicitly asks.
- Do not move French content outside `TCF Canada French`.
- Preserve original source files.
- Make focused changes and explain uncertain interpretations.
- If a file has user edits, work with them instead of overwriting them.

## Cross-Device Workflow

When continuing this project on another device:

1. Open the synced Obsidian vault in Codex.
2. Read `TCF Canada French/French Notes Agent Handoff.md`.
3. Use the handoff to update the existing `TCF Canada French/AGENTS.md`.
4. If `AGENTS.md` does not exist, create exactly one `AGENTS.md` inside `TCF Canada French`.
5. Before editing French notes, read `AGENTS.md` and the target note/source file.
6. When the user has taken another French class, treat the textbook PDF as newly updated through Obsidian Sync and extract the relevant lesson material into notes from the latest PDF annotations.
7. If the user replaces the annotated textbook PDF with a newer file/version, update affected note links so their PDF wikilinks still open the latest textbook and the intended pages.
8. Run a complete link sweep across all lesson notes after every replacement; do not assume lessons untouched in the current update already point to the newest PDF.
