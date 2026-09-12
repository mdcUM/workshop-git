# 👋 Welcome to Tech Dev!

This is where all Tech Dev members live.

By the end of this exercise, your profile will be in this repo alongside everyone
else's — and you'll have gone through the full Git + GitHub workflow we just covered
on the slides.

> **Before you start:** make sure you have Git installed and a GitHub account ready.
> If you don't have one, make one at [github.com](https://github.com) — it's free.

---

## What you'll do

```
clone the repo  →  create a branch  →  add your profile  →  commit & push  →  open a PR
```

---

## Step 1 — Clone the repository

Download a copy of this repo to your computer.

```bash
git clone https://github.com/<org>/techdev-crew.git
cd techdev-crew
```

You now have the full repo on your machine. Run `ls` to see the files.

---

## Step 2 — Create your branch

**Never work directly on `main`.** Create a branch just for your changes.
Use the format `member/firstname-lastname` (all lowercase, hyphen between names).

```bash
git checkout -b member/jane-doe
```

You're now on your own branch. Changes here won't affect `main` until your PR is merged.

To double-check which branch you're on:

```bash
git branch
```

The branch with a `*` next to it is the active one.

---

## Step 3 — Copy the template

Make a copy of the profile template and name it after yourself.
Use the same `firstname-lastname` format, keeping the `.md` extension.

**Mac / Linux:**
```bash
cp members/_template.md members/jane-doe.md
```

**Windows (Git Bash):**
```bash
cp members/_template.md members/jane-doe.md
```

**Windows (Command Prompt):**
```cmd
copy members\_template.md members\jane-doe.md
```

---

## Step 4 — Fill out your profile

Open your new file in VS Code and answer the questions inside it.

```bash
code members/jane-doe.md
```

Check out `members/example-techdev-bot.md` if you want to see what a finished
profile looks like.

---

## Step 5 — Stage your file

Tell Git you want to include your new file in the next commit.

```bash
git add members/jane-doe.md
```

Check that Git has registered it:

```bash
git status
```

You should see your file listed under *"Changes to be committed"* in green.

---

## Step 6 — Commit your changes

Save a snapshot of your changes with a short, descriptive message.

```bash
git commit -m "Add Jane Doe to members"
```

Good commit messages complete the sentence: *"If applied, this commit will..."*
→ *"If applied, this commit will **Add Jane Doe to members**"* ✅

---

## Step 7 — Push your branch to GitHub

Send your local branch up to the remote repo.

```bash
git push origin member/jane-doe
```

After pushing, Git will print a link directly to open a Pull Request. You can
click it, or follow Step 8 below.

---

## Step 8 — Open a Pull Request

1. Go to the repo on GitHub: `https://github.com/<org>/techdev-crew`
2. You'll see a yellow banner: **"member/jane-doe had recent pushes — Compare & pull request"**. Click it.
3. Give your PR a title like `Add Jane Doe to members`
4. Add a fun comment in the description if you want
5. Click **"Create pull request"**

That's it! An officer will review and merge it.

---

## ✅ Checklist

- [ ] Cloned the repo
- [ ] Created a branch named `member/firstname-lastname`
- [ ] Copied `_template.md` to `members/your-name.md`
- [ ] Filled out your profile
- [ ] Staged your file with `git add`
- [ ] Committed with a descriptive message
- [ ] Pushed your branch
- [ ] Opened a Pull Request on GitHub

---

## 🏃 Done early? Try these bonus challenges

**1. Watch the branch tree grow**
After a few people have pushed, run this to see the live branch graph:
```bash
git fetch --all
git log --all --oneline --graph
```

**2. Explore your changes**
See exactly what you changed compared to `main`:
```bash
git diff main
```

**3. Improve the template**
Think the profile questions could be better? Edit `members/_template.md` and
open a PR for that too. *(Warning: if two people do this at the same time, you
might get a merge conflict — a great thing to experience in a safe environment!)*

**4. Read the CONTRIBUTING guide**
Check out `CONTRIBUTING.md` for more on how real teams structure their Git workflow.
