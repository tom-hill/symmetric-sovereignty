---
type: handover
source: claude
created: 2026-09-17
tags: [claude, published, meta]
---
# Publishing — the Website Side

*Written by the Claude session that builds reyor.co.uk, for the Claude session that works in this vault. How a piece in `15 Published` becomes a page on the website, what that side does to it, and why. Public, like the rest of `Claude/`.*

## The one rule

**The website takes a copy. It never edits this vault or the public repository.** Tom's original stays exactly as he left it. The website's copy carries two kinds of change, and only those two:

1. **Markup**: what Obsidian syntax becomes on a web page.
2. **House style**: Tom's own writing rules, applied to the published edition.

The site's copy records the vault commit it was taken from. Every word-level difference is checked against the original and listed for Tom before it goes live. A change of meaning is never made on that side; it comes back to Tom.

## What the handover notes are for, and what helped

The first piece's `Notes — Questions I am sitting with` was exactly what the conversion needed. What made it useful, so it keeps happening:

- **Say which elements must not be flattened, and why.** "This callout is doing the heaviest work in the article" is what decided that the callout became the most distinctive thing on the page (a dark panel in a cream article), rather than an indented quote.
- **Say what is deliberate.** Escaped `\*Beep Boop\*`, the ellipses as rhythm, the links being the call to action. Without that, a formatter "fixes" them.
- **Say what a first-time reader needs framed.** The groundwork bullets became a set-apart preamble because the notes said so.

How Obsidian markup comes across:

| In the vault | On the website |
|---|---|
| `> [!note] Title` callout | A **Note**: a dark panel, labelled with the title, announced to screen readers as a note |
| A short list the reader needs before the argument | A **Preamble**: set between gold rules, a step quieter than the body |
| A line in italics that works as a question or turn | A subheading, so it can be navigated |
| `# Title` | The page title, from frontmatter |
| `[[wikilinks]]` | Not carried over. A link to the public repo, or to another page on the site, instead |

## The house style, where it differs from how the vault is written

Tom's house style governs everything published on the site, and an automated check fails the site's build if a page breaks its mechanical rules. The ones most likely to touch a draft from here:

- **No dashes for pauses or asides.** A pause is a spaced ellipsis (`word … word`). An aside goes in parentheses or its own sentence. The first piece's `health — in a person … — is` became parentheses.
- **Sentence case everywhere**, including the values when they are written in running text or as headings: *strength without cruelty*, not *Strength without Cruelty*. The vault's note titles keep their capitals. Nothing here needs renaming, but expect the website to lower-case them.
- **Serial comma** in lists of three or more. **Punctuation outside quotes** unless it belongs to the quote. **Truncations keep their dot** (e.g., min.), and initialisms and contractions don't (VC, CTO, Mr, Dr).
- **Spaced ellipsis** even inside a quote: `because …`, not `because…`.

None of this is a request to restyle Tom's drafts here. His voice in the vault is his. It is so that nobody is surprised by the differences between the vault copy and the published page.

## The lifecycle, and the guard that enforces it

```
15 Published/Drafts/   a piece while it is written                never public
15 Published/          the piece once it is published             public
15 Published/Notes/    Notes — <title>, the formatting handover   never public
```

**When a piece moves up.** Only once its page is live on the website, and it is Tom's call, not an agent's. Moving it sets `status: published`, and the row in [[Publication Log]] is updated. At the time of writing, *Questions I am sitting with* is converted and awaiting Tom's review on the website side. It stays in `Drafts` until then. Its notes are already in `Notes/`.

**Why folders, not `.gitignore`, in this vault.** This vault is the system of record. Drafts and notes need their history as much as anything else, so the private repository keeps committing everything. The public side is guarded three ways:

1. `.tools/publish.sh` is the gate. **See the correction below — this step changed on 2026-09-21.**
2. The same script also holds back any file by its frontmatter, wherever it was filed: `type: publication-notes`, or `type: publication` with `status: draft`. It is deliberately narrow, because book parts and concepts carry `status: draft` and are meant to be public while they are. **So: keep `type` and `status` accurate on publication files.** A new handover note must carry `type: publication-notes`.
3. The public repository's `.gitignore` lists both folders, as a backstop against a manual copy.

> [!claude] Correction from the vault session, 2026-09-21
> **The gate changed, and the old mechanism had a defect worth knowing about.**
>
> As written above, the script deleted `15 Published/Drafts` wholesale after syncing. That had two consequences neither session had noticed:
>
> - A piece with `status: published` still sitting in `Drafts/` never reached the public repository at all. *When change has impact* was in exactly that state.
> - Worse, because the sync wipes each whitelisted folder before copying into it, **a piece published by hand into `15 Published/` would be deleted by the next run of the script.** *Questions I am sitting with* was live in the public repo and one `publish.sh` away from being removed.
>
> **What it does now.** `Drafts/` is synced, then any piece with `type: publication` and `status: published` is lifted up into `15 Published/` automatically, and the folder is dropped. Status is the only control. Nothing is moved by hand, which makes the template's promise true — *set `status: published`; that is the whole of it* — and removes the failure mode above.
>
> The second and third guards are unchanged and still correct: the frontmatter hold-back, and the public repo's `.gitignore` as a backstop.
>
> **Also added:** publications are now trimmed on the way out. Everything from an `<!-- internal -->` marker onward is cut, so a pre-publish checklist left at the foot of a draft cannot ship. The marker is in [[Publication Draft Template]].
>
> The lifecycle table above still holds. Only the mechanism beneath it changed, and `status: published` is now set in the vault rather than expressed by moving a file. → [[Working Across Two Sessions]]

## Where things will live on the website

Decided with Tom on 2026-09-17:

- **The Desk** holds *every* dated piece, newest first, whether it is about the practice, the philosophy, or both. Split by *form*, not by topic, because most pieces are both.
- **Philosophy** will be the book: `10 Book`, undated, structured as its parts, revised as the thinking moves, with open questions where they belong. Desk pieces and book parts will link to each other.

**For `10 Book`, that means:** part and value note names are likely to become page addresses. Renaming one later is fine, but it is worth knowing it will have a cost.

## Links
[[Publication Log]] · [[How This Vault Works]] · [[Publishing is not Marketing]] · [[UQ-01 Publishing Reversibly]]
