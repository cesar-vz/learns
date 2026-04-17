# 🔶 GitHub Sync Guide — VS Code

> `▓▒░` _multi-machine sync protocol_ `░▒▓`

---

## 🔸 Golden Rule · Multi-Machine

*   **Pull before you start. Push when you finish.**
*   Skip the pull → you edit stale code → merge conflicts incoming ⚠

---

## 🟠 Best Default · `Commit & Sync`

You work across **two machines** → make **Commit & Sync** your default.

### 🔸 What it does — one click

1.  **Commits** your changes locally
2.  **Pulls** new changes from GitHub
3.  **Pushes** your commits to GitHub

### 🔸 Why it fits your setup

*   Auto-handles both directions — zero forgotten pulls
*   Both laptops stay mirrored
*   One button, three operations

### 🔸 Set it as default

1.  Open **Source Control** panel in VS Code
2.  Click the `⌄` arrow beside the **Commit** button
3.  Select **Commit & Sync**
4.  Main button now runs Commit & Sync every time

---

## 🔶 The 4 Core Actions

| Glyph | Action | Function |
| --- | --- | --- |
| ⬇ | **Clone** | Pull a repo to a new machine — once per machine |
| ● | **Commit** | Snapshot **locally** — GitHub untouched |
| ▲ | **Push** | Upload local commits to GitHub |
| ▼ | **Pull** | Download latest from GitHub |

**Mental model**

```
Commit → save locally
Push   → send to remote
Pull   → receive from remote
Sync   → pull + push combined
```

---

## 🔶 Commit Dropdown Decoded

| Option | Behavior |
| --- | --- |
| **Commit** | Local only · GitHub untouched |
| **Commit (Amend)** | Merge into previous commit |
| **Commit & Push** | Commit + upload · solo, single machine |
| **Commit & Sync** 🟠 | Commit + pull + push · **your default** |
| **Commit & Create PR** | Team collaboration flow |

---

## 🔶 Daily Workflow — 2 Computers

### ▸ Session start

*   Launch VS Code
*   Check status bar → `⇣1 ⇡0` means pull pending
*   Pull first _(or let Commit & Sync handle it)_
*   Edit

### ▸ Session end

*   Write a clear commit message
*   Hit **Commit & Sync**
*   Close lid

---

## 🟠 Status Bar Shortcut

Bottom-left of VS Code displays:

```
 main  ⇣1 ⇡2
```

*   **⇣N** → commits pending pull
*   **⇡N** → commits pending push
*   Click the area → syncs both directions instantly

---

## ⚠ The One Scenario to Avoid

**Editing the same file on both machines without pushing in between.**

```
✗ Mon  · edit laptop A · forget to push
✗ Tue  · edit same file on laptop B
✗ Wed  · push from A → ⚡ merge conflict
```

**Prevention** → always `Commit & Sync` before closing the lid. Treat it like saving.

---

## 🔶 New Machine Setup Checklist

*   ☐ Install VS Code
*   ☐ Sign in to GitHub
*   ☐ **Clone** the existing repo _(don't create a new one)_
*   ☐ Open the cloned folder
*   ☐ Set **Commit & Sync** as default
*   ☐ Start editing