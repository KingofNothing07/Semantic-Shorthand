---
name: semantic-shorthand-language
description: Teaching file for the Semantic Shorthand language only — notation, symbols, syntax, expressions, core concepts, compression, and Rosetta Stone. Fully usable standalone for reading and writing the notation. Excludes logging practice, curation workflows, and Coding Mode.
---

# Semantic Shorthand Language and Grammar
Version 01.01-language

**Purpose.** This file teaches the Semantic Shorthand language itself: how to read and write expressions, the symbols and their meanings, syntax rules, core concepts, and the standard compression method. It is a teaching reference only and is fully usable on its own for the language. It does not cover logging practices, curation, inheritance packaging, or Coding Mode.

**Format note.** Notation lives in fenced code blocks so operators remain literal. When writing actual expressions in Markdown, wrap them in fences to prevent reformatting. Disable autocorrect in rich-text tools.

**Read Gate.** This is a pure language reference. No activation or logging behavior is implied.

---

# Foundations

## Hard Rules (must be followed)

1. Expressions follow correct left-to-right syntax.
2. Subjects, attributes, interactions, decisions, reasoning, relationships, conditional paths, dependencies, and outcomes are preserved for accurate reverse translation.
3. Nested comments are the only form of inflation.
4. The in-line expression holds the current latest-approved version. A superseded version moves to a nested comment with `::vN`; the new version replaces it in-line. Reverse translation uses the in-line version unless a specific earlier version is requested.
5. The `-` symbol (remove/subtract) is always spaced between terms, never attached. Attached `-x` is reserved for a negative number inside M. Semantic negation uses `!` only. This distinction is load-bearing.
6. The `^n` loop/repeat suffix attaches only to a closing grouping delimiter (`)`, `]`, `}`) or a Special Set reference. It never attaches to a bare number/variable or to a parenthetical of standalone math outside M. Those remain ordinary exponentiation; write them under M if needed. This distinction is load-bearing.

## Soft Rules (strongly recommended)

1. Default to stacking when readable on one line.
2. Prefer nested material below the related expression.
3. Use standard compression by default. Wrap exact text in `||...||`. Loosen or tighten only on request.
4. Use sub-modifiers only for meaningful precision.
5. Use `(p:%)` only when probability matters. Derive other forms from it plus `?` or `~`.
6. Modified symbols must remain intuitive; explain non-intuitive ones with a nested comment.
7. Create Special Sets primarily on user request or after asking on clear reuse. Check for Name collision.
8. Capitalize the Subject as a scannability convention (proper nouns keep natural casing).
9. Prefer a bookended pattern (`2, 4, 6, ..., 20`) over `Hn` when the end is easy to state. Reserve `Hn` for non-trivial endpoints.

## Notation Reference

Read the block below as literal notation.

```
Prefixes
:         Expression signifier. Begins every expression. Followed directly by the Subject (or grouped Subjects). Example: :Project, status (active)
?         Uncertain/unknown. Example: ?:Active
~         Approximate. Example: ~50%
::Name    Special Set. Example: ::CoreTeam:(Alice + Bob + Cara)
M         Math mode. Forces mathematical reading of symbols inside the segment. Example: M:E = mc^2 or :Energy, M(E = mc^2)

Logic
+         Join/AND. Example: cereal + milk
-         Remove/subtract (spaced). Example: Group - Mary
,         Loose succession / separator. Weakest order strength.
|         OR. Example: A | B
!         NOT/negation. Example: !:Approved

Conditionals / Flow
->        Then/sequence. Example: Research -> Analysis
->>       Becomes/transitions to. Example: design ->> prototype
>>        Requires/depends on (dependent first). Example: Approval >> Budget
><        Else/alternative. Example: continue >< turn back
<->       Biconditional. Example: Ready <-> Checks passed
;         Lambda (Input;Output). Example: :Fuel;Drive
!=        Does not meet/not equal.
<= >=     Inclusive comparison.

Grouping & Hierarchy
( ... )   Innermost/basic set.
[ ... ]   Intermediate set.
{ ... }   Outermost set.
||...||   Absolute/Invariant. Exact content that must not be altered or paraphrased. Example: ||2026-09-15|| or :Yoda, quote ||Do or do not, there is no try.||
H         Hierarchy/order prefix. Strongest order strength. Example: H:(1: Research, 2: Design, 3: Build)
Hn        Pattern step count (bare number on H). Example: H10(2, 4, 6, ...)
...       Continuation of pattern / open range. Example: 2, 4, 6, ..., 20

Loops
^n        Loop/repeat the enclosed unit n times from the start. Attaches only to closing delimiter or Special Set. Example: (:Boy, baseball, hit -> run)^2

Wraps / Comments
"..."     External Reference (name/identifier only).
'...'     External Reference Summary (pairs with the above; may carry disposition tag).
// ... // General comment.

Suffixes & Sub-Modifiers
::vN      Version suffix (inside nested comment).
(p:%)     Probability. Example: success (p:85%)
(t:...)   Time/duration.
(d:n)     Dimensions/layers.
(co:...)  Coordinates.
```

## Notation: Symbols and Syntax

A well-formed expression reads left-to-right as a compressed version of the original meaning. Compression re-encodes; it does not discard essential detail.

1. Every expression begins with `:` followed by the Subject.
2. Readable Flow: structure so left-to-right reading reconstructs meaning with minimal reordering.
3. Special Set: `::Name:` followed by contents. Shared Names join into one set. Reference later by `::Name`.
4. Set hierarchy: `( )` basic, `[ ]` intermediate, `{ }` outermost. Use only levels needed.
5. `H` marks ordered content. `1:Name` inside H is a correlator only. `Hn` sets total steps for a `...` pattern.
6. `M` forces mathematical interpretation inside its segment only. No keyboard restriction inside M.
7. `||...||` preserves exact content. Not inflation.
8. Symbols may be combined when the result stays intuitive and left-to-right readable. Non-intuitive combinations require a nested comment.
9. Sub-modifiers live inside parentheses and attach to a subject, attribute, or modifier.
10. Stacking (commas and operators on one line) is the default when readable.
11. `...` continues a clear pattern (leading, mid-list, or open).
12. The three wraps are the only inflation devices. `||...||` is not one of them.
13. Left-to-right is the default order.
14. `^n` restarts a complete enclosed unit n times. Distinct from `Hn` (which grows one progression).

Shared-subject compression: `:(Sally + Mark) -> store, buy (shoes)` preserves every subject and outcome while stating the shared part once.

## Core Concepts

An expression is a self-contained statement beginning with `:` (or prefix + colon) followed by the Subject.

Minimum: `:Subject`  
Typical: `:Subject, attribute (modifier)`  
Conceptual: `:Subject, attribute (modifier (sub-modifier)) + related -> consequence`

Factors: Subject (position after colon), Attribute (quality/status), Modifier (further description), Sub-modifier (extra precision, recursive). Phrasing is flexible; the same fact can be arranged differently and still reverse-translate correctly if Hard Rules are followed. High-fidelity reconstruction is primary; token savings is secondary.

Readable Flow Principle: the expression should already read as a coherent compressed sentence.

Stacking is preferred because it mirrors left-to-right reading order.

Two kinds of nesting:
- Structural (indentation under a title) shows belonging; not inflation.
- Comment/wrap nesting attaches notes, versions, or references; must use one of the three wraps.

**Absolute/Invariant (`||...||`).** Exact-fidelity content, not a comment. Two primary uses: fixed values that must not drift, and short exact-replication blocks. The attribute word before a quoted Absolute is required so reverse translation knows what the exact text is. Keep blocks short. Works inside M.

**Hierarchy (`H`).** Marks ordered content evaluated left-to-right. `Hn` sets the total steps of a `...` pattern.

**Math Mode (`M`).** Forces mathematical interpretation of symbols inside its segment only. Ordinary algebra works unchanged. Subjects and Attributes can name equations (word-problem style). Unicode and math notation are allowed. Example: `:Energy, M(E = mc^2)`. Inside M, system flow operators are read as math first unless surrounding context clearly requires otherwise.

**Currying / Chaining.** The result of one expression becomes the input of the next via flow operators. Produces readable process paths while preserving relationships. Example:  
`:Requirements complete -> Design phase begins -> Development start >> Design approved`.

**Combinatorial Freedom.** Any intuitive combination of existing symbols is allowed. Examples of derived forms: `!+` (NAND), `!|` (NOR), `!<->` (XOR), `~p:%`, `!(...)`, `?>>`, `~->`. Non-intuitive combinations need a nested comment that includes the reverse-translation line.

**Special Sets (`::Name`).** Named reusable collections created with `::Name:` followed by contents. Shared Names join automatically (including across logs). Reference later by `::Name`. Before creating, check for an existing Name; if one exists, ask whether to join or use a suffix. They can also serve as version caches. Example:  
`::CoreTeam:(Alice + Bob + Cara)` then later `:Review >> ::CoreTeam`.

**Versioning.** The in-line expression is always the current latest-approved version. Superseded content moves to a nested `::vN` cache. Unapproved ideas are ordinary comments without version numbers. Parallel alternatives can be held as equal-standing `::vN` entries; swapping which is in-line is a lightweight curation action. A version note describes what changed.

**External References.** Two forms:  
`"Name or identifier only"` — pointer only.  
`'Summary of the referenced material (disposition: attach)'` — pairs with the name-only form and may carry a disposition tag.

## Compression & Practice

Compression removes filler only. Sacred content is re-encoded with symbols and structure, never discarded. Reconstructibility is non-negotiable.

### Rosetta Stone — Standard Compression

Raw paragraph  
The hiring committee evaluated four finalists for the Head of Engineering role and selected Candidate R. The decision rested on her proven ability to scale teams, strong system-design background, and clear alignment with the company's remote-first culture. There is remaining uncertainty about her willingness to relocate for the quarterly on-sites. If she declines relocation, the committee will move to Candidate T and reopen the compensation band. No offer letter can be sent until both reference checks and the executive interview loop are complete. Reference checks are scheduled for Thursday; the final executive panel is set for the following Tuesday. Supporting material is filed as "Head of Engineering Finalist Packet — August".

Standard compression  
```
:Hiring committee, 4 finalists -> Candidate R (Head of Engineering)
:R, reason (scale teams + system-design background + remote-first culture alignment), relocation (? quarterly on-sites)
:Declines -> T + reopen compensation
:Offer letter >> reference checks + executive loop
:Reference checks (Thursday) + Executive panel (following Tuesday)
"Head of Engineering Finalist Packet — August"
```

Reverse translation  
The hiring committee evaluated four finalists and selected Candidate R for Head of Engineering. Reasons: scale teams, system-design background, and remote-first culture alignment. Relocation for quarterly on-sites is uncertain; if declined, move to T and reopen compensation. Offer letter requires reference checks and the executive loop. Reference checks Thursday and executive panel the following Tuesday. Supporting material: "Head of Engineering Finalist Packet — August".

Standard compression is the only taught method. It can be written looser (expanded phrasing) or tighter on explicit request. Fidelity first, tokens second. Absolute/Invariant is used for any text that must not drift.

Clarifying examples:
- Shared-subject: `:(Sally + Mark) -> store, buy (shoes)`.
- Dependency with flow: `:Offer letter >> reference checks + executive loop`.
- Uncertainty marker: `relocation (? quarterly on-sites)`.
- External reference name-only: `"Head of Engineering Finalist Packet — August"`.

## Glossary (Language Terms)

Attribute — quality, status, or component of a Subject.  
Standard Compression — stacking and symbols with every sacred element preserved; verbatim text in `||...||`.  
Absolute / Invariant — material in `||...||` that must not be altered.  
Currying / Chaining — using one expression's result as the next's input.  
Expression — basic unit beginning with `:` followed by the Subject.  
Factors — Subject, Attribute, Modifier, Sub-modifier.  
Hierarchy (H) — prefix for ordered content.  
Hierarchy Step Count (Hn) — bare number on H setting total steps of a `...` pattern.  
Inflation — added material beyond the core expression; only nested comments/wraps are allowed.  
Loop / Repeat Suffix (`^n`) — repeats an enclosed unit n times from the start.  
Math Mode (M) — prefix forcing mathematical interpretation inside its segment.  
Modifier — further description of an attribute.  
Nesting — structural (indentation) or comment/wrap.  
Phrasing — writing data into valid expressions while preserving necessary detail.  
Readable Flow Principle — left-to-right reading reconstructs intended meaning with minimal reordering.  
Sacred Content — subjects, attributes, interactions, decisions, reasoning, relationships, conditional paths, dependencies, outcomes.  
Special Set (`::Name`) — named reusable collection.  
Stacking — linking related content on one line with commas and operators.  
Sub-modifier — extra precision nested inside a Modifier.  
Subject — main focus; defined by position after the colon.  
Versioning / Version Cache — in-line holds current; superseded versions move to nested `::vN`.  
Wraps / Comments — `"..."`, `'...'`, `//...//` (the only inflation forms).  
External Reference — name-only quote or summary quote (may carry disposition).

---

# END OF LANGUAGE AND GRAMMAR FILE

This file covers the notation and language only and is fully usable on its own for reading and writing expressions. Logging, curation, inheritance packaging, and Coding Mode are excluded by design.
