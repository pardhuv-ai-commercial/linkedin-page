# How to publish a new piece on The Deployment Gap

A simple reference for the two tasks you'll do repeatedly:
1. **Promote a "Coming next" row to a published entry**
2. **Add a brand new upcoming topic to the pipeline**

---

## Task 1 — Publish a new piece (most common task)

When you have a finished HTML file ready to go live, you do **two things**:

### Step A — Upload your new HTML file to the repo root

Name it cleanly with hyphens, no spaces:
```
mas-governance-guide.html
multi-party-support-case-study.html
agentic-roi-framework.html
```

### Step B — Edit `index.html` in two places

Open `index.html` and find this block (around line 307):

```html
<!-- UPCOMING PLACEHOLDERS — add new rows above this block as you publish -->
<div class="pub-upcoming">
  <div><span class="upcoming-label">Coming next ·</span><span class="upcoming-title">Agentic AI Governance for APAC Financial Institutions — MAS MGF Practitioner Guide</span></div>
  <span class="upcoming-status">In research</span>
</div>
```

**Replace that entire `<div class="pub-upcoming">` block** with this published row template:

```html
<a href="YOUR-FILENAME.html" class="pub-row">
  <div class="pr-num"><div class="prn">05</div></div>
  <div class="pr-body">
    <div class="prs">YOUR SERIES NAME · 2026</div>
    <div class="prt">YOUR FULL TITLE HERE</div>
    <div class="prd">A 1–2 sentence description of what this piece covers and who it's for.</div>
  </div>
  <div class="pr-arr">→</div>
</a>
```

Fill in:
| Placeholder | What to put |
|---|---|
| `YOUR-FILENAME.html` | The exact filename you uploaded, e.g. `mas-governance-guide.html` |
| `05` | The next publication number |
| `YOUR SERIES NAME · 2026` | e.g. `Governance · 2026` or `Case Study · 2026` |
| `YOUR FULL TITLE HERE` | The title as it appears in the HTML file |
| Description | 1–2 sentences from your intro paragraph |

Then push `index.html` alongside the new HTML file. Done — live within 60 seconds.

---

## Task 2 — Add a new topic to the pipeline

When you want to signal a future piece without publishing it yet, add a new `pub-upcoming` row.

Find the last `pub-upcoming` block in `index.html` and paste this **after** it:

```html
<div class="pub-upcoming" style="border-top:none">
  <div><span class="upcoming-label">Coming next ·</span><span class="upcoming-title">YOUR TOPIC TITLE HERE</span></div>
  <span class="upcoming-status">In research</span>
</div>
```

Status options (swap the text inside `upcoming-status`):

| Text | When to use |
|---|---|
| `In research` | Just started — gathering sources |
| `Drafting` | Writing in progress |
| `Agent review` | AI agent team is running |
| `Final edit` | Almost ready — your review pass |

---

## Task 3 — Update the README.md publication table

Each time you publish, update the matching row in `README.md`:

Change:
```markdown
| 05 | Agentic AI Governance for APAC Financial Institutions | Governance | 🔬 In research |
```

To:
```markdown
| 05 | [Agentic AI Governance for APAC Financial Institutions](mas-governance-guide.html) | Governance | ✅ Published |
```

---

## The two-file push (every publication)

Every new piece = exactly **two files pushed** to your repo root:

```
1.  your-new-piece.html     ← the article itself
2.  index.html              ← updated with the new pub-row entry
```

Optionally update `README.md` at the same time.

GitHub Pages rebuilds automatically. No build commands. No config. ~60 seconds.

---

## Status badge quick reference

Copy-paste the status text that matches where your piece is:

```
In research
Drafting  
Agent review
Final edit
```

---

## File naming convention

| Do | Don't |
|---|---|
| `mas-governance-guide.html` | `MAS Governance Guide.html` |
| `multi-party-case-study.html` | `multi party case study v2 FINAL.html` |
| `agentic-roi-framework-2026.html` | `new article.html` |

Lowercase, hyphens only, no spaces, no version numbers in the final name.

---

## Your current site map

```
index.html                    ← Homepage (edit this each time you publish)
about.html                    ← About page (edit only when your bio changes)
fi-agentic-stack.html         ← Publication 01 ✅
agent-native-data-layer.html  ← Publication 02 ✅
context-window.html           ← Publication 03 ✅
format-selection.html         ← Publication 04 ✅
README.md                     ← Repo description (update publication table)
```
