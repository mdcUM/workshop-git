# Git Workshop

This is a small repo with profiles of each MDC newbie.

By the end of this exercise, your profile will be in this repo alongside everyone
else's — and you'll have gone through the full Git + GitHub workflow we just covered
on the slides.

## Steps in this tutorial

1. clone the repo
2. create a branch
3. add your profile
4. commit & push
5. open a PR


## Step 1 — Clone the repository

Download a copy of this repo to your computer.

```bash
git clone https://github.com/mdcUM/workshop-git
cd workshop-git
```

---

## Step 2 — Create your branch

Create a branch just for your changes.
Use the format `member/firstname-lastname`.

```bash
git checkout -b member/firstname-lastname
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

**Mac / Linux/ Windows Git Bash**
```bash
cp members/_template.md members/firstname-lastname.md
```


**Windows (Command Prompt):**
```bash
copy members\_template.md members\firstname-lastname.md
```

---

## Step 4 — Fill out your profile

Open your new file in VS Code and answer the questions inside it.

```bash
code members/firstname-lastname.md
```

(Or just open in another text editor)

---

## Step 5 — Stage your file

Tell Git you want to include your new file in the next commit.

```bash
git add members/firstname-lastname.md
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
git commit -m "Add Firstname Lastname to members"
```

---

## Step 7 — Push your branch to GitHub

Send your local branch up to the remote repo.

```bash
git push origin member/firstname-lastname
```

After pushing, Git will print a link directly to open a Pull Request. You can
click it, or follow Step 8 below.

---

## Step 8 — Open a Pull Request

1. Go to the repo on GitHub: `https://github.com/mdcUM/workshop-git`
2. You'll see a yellow banner: **"member/firstname-lastname had recent pushes — Compare & pull request"**. Click it.
3. Give your PR a title like `Add Firstname Lastname to members`
4. Add a comment in the description if you want
5. Click **"Create pull request"**
