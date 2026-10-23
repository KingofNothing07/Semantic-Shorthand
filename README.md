# Semantic Shorthand

**High-fidelity, low-token inheritance logs that survive across AI sessions, models, and agents.**

Semantic Shorthand is a structured note-taking and context-preservation system designed for AI collaboration. It lets you capture decisions, reasoning, relationships, conditionals, dependencies, and outcomes in a compressed but fully reconstructible form so that a later reader — human or AI — can continue the work without rediscovery or the usual summarization loss.

Unlike ordinary chat summaries or free-form notes, Semantic Shorthand treats certain content as sacred. Compression re-encodes that content; it never discards it. Only explicitly approved material enters the main log. The result is a living context engine that stays accurate, scannable, and token-efficient over long-running projects, multi-session work, and agent hand-offs.

---

## Purpose

Most AI conversations lose critical detail the moment context is summarized or the session ends. Semantic Shorthand solves this by giving you:

- A consistent notation that LLMs can read and write with high fidelity.
- An approval discipline so exploratory ideas stay separate from the official record.
- Versioning and curation so the current authoritative state is always clear.
- Reverse translation into natural language (or other forms) so the log can be handed to anyone.
- Optional Coding Mode for software design logs that can guide implementation.

The north star is inheritance: a future session, a different model, or another agent should be able to pick up the work with a clear picture of what was decided, why, what is still open, and how pieces relate.

---

## Core Abilities

| Ability | What it does |
|---------|--------------|
| **High-fidelity compression** | Re-encodes decisions, attributes, relationships, conditionals, dependencies, and outcomes using a small set of symbols while preserving reconstructibility. |
| **Approved-data discipline** | Only material you explicitly accept enters the main log. Exploratory ideas stay in nested comments until approved. |
| **Versioning & curation** | The in-line expression is always the current approved version. Superseded versions move to a nested cache (`::vN`). Parallel alternatives can be held and swapped. |
| **Special Sets** | Named reusable collections (`::Name`) that can be referenced later and automatically join when the same name is used. |
| **Reverse translation** | Turns the shorthand log back into clear natural language (or other styles) built strictly from the official log. |
| **Inheritance packaging** | Produces a ready-to-hand-off document with front-matter, status, and reconstruction guidance. |
| **Coding Mode** | Specialized structure for software design: flow/intent (sacred) separate from implementation (versionable), with scope-aware regression checks. |
| **Math Mode & Absolute content** | `M` forces mathematical reading; `||...||` preserves exact text that must not drift. |
| **Cross-session / multi-agent continuity** | Logs are designed to be picked up by a different model or agent with a brief status acknowledgment. |

---

## Why Use Semantic Shorthand

- **Session survival** — Context does not evaporate when you start a new chat or switch models.
- **Token efficiency with fidelity** — Far lower token cost than raw transcripts, without the lossy nature of typical summaries.
- **Honest record** — Clear separation between approved decisions and exploratory ideas.
- **Readable by humans and AIs** — Left-to-right expressions that reverse-translate cleanly.
- **Scales with complexity** — Useful for simple decision logs and for multi-component software or multi-agent systems.
- **Lite version available** — Same power at lower token cost when you need it.

Ordinary notes or AI summaries often flatten conditionals, drop dependencies, or silently promote unapproved ideas. Semantic Shorthand makes those distinctions explicit and enforceable.

---

## How to Install and Use with AI

### Quick Install
1. Choose the file that matches your need (see the table below).
2. Copy the **entire** contents of that file.
3. Paste it into your AI as:
   - System prompt / custom instructions, or
   - Project knowledge / knowledge base, or
   - Skill upload (if your platform supports skill files).

### Activation Notes
- Loading the file does **not** automatically force every response into log form.
- The skill activates when you explicitly request a Semantic Shorthand log, inheritance package, curated Delta, or invoke the skill by name.
- Ambiguous requests get one clarifying question rather than silent assumption.
- Outside an active request the AI behaves normally.

### Practical Tips
- Use plain text or fenced Markdown. Several symbols (`#`, `*`, leading `-`, `_`) can be altered by rich-text editors or autocorrect.
- Disable autocorrect when writing real logs.
- After a package is produced, review it and correct anything missing or incorrect before treating it as final.
- For mid-session or retroactive logs, the system expects an outline first and approval before the full log is written.

### Choosing a File
- Want the complete guided system? → Full package or Lite.
- Just learning or writing the notation? → Language & Grammar.
- Already know the notation and want logging/curation practice? → Logging, Curation & Inheritance.

---

## Files — Detailed Descriptions

| File | What it contains | Best for | Token profile |
|------|------------------|----------|---------------|
| [`01.01_Semantic_Shorthand-Skill_Package.md`](01.01_Semantic_Shorthand-Skill_Package.md) | Full skill package: skill prompt, complete language teaching document, and full logging/curation/inheritance teaching document (including Coding Mode). | Users who want maximum guidance and the complete system in one file. | Higher |
| [`0.1.01_Semantic_Shorthand_lite.md`](0.1.01_Semantic_Shorthand_lite.md) | Fully capable lite version of the skill package. Equivalent ability to the full package (language + logging + Coding Mode) written more concisely. | Everyday use and token-conscious sessions. Recommended starting point for most people. | Lower |
| [`Semantic_Shorthand_Language_and_Grammar.md`](Semantic_Shorthand_Language_and_Grammar.md) | Language and notation only: symbols, syntax, Hard/Soft Rules, Special Sets, Math Mode, Absolute/Invariant, currying, compression, Rosetta Stone, and glossary. No logging workflow or Coding Mode. | Learning the notation, quick reference, or using the language standalone. | Low |
| [`Semantic_Shorthand_Logging_Curation_Inheritance.md`](Semantic_Shorthand_Logging_Curation_Inheritance.md) | Practice document only: starting logs (clean and retroactive), approved-data capture, Delta curation, versioning, Special Sets in practice, reverse translation, inheritance packaging, and Coding Mode. Assumes the language is known. | Users who already understand the notation and want the operational guidance. | Medium |

Examples of the notation in use (including the Rosetta Stone) appear inside the teaching documents themselves.

---

## License

MIT — free to use, modify, and share. See [`LICENSE`](LICENSE).

---

Questions, corrections, or improvements are welcome via issues or pull requests.