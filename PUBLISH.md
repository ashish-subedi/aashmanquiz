# Publishing this to GitHub Pages

The folder `gk-quiz-site` is already a git repository with one commit on branch
`main`. You only need to point it at a GitHub repo and push.

---

## Option A — no command line (easiest)

1. Go to <https://github.com/new>.
   Name it e.g. **gk-quiz**, set it to **Public**, and do **not** tick
   "Add a README" (the folder already has one).
2. On the new empty repo page click **uploading an existing file**.
3. Drag in these files from `AM Preparation\gk-quiz-site`:
   - `index.html`
   - `README.md`
   - `question_bank.json`
   - `.nojekyll`   ← if Windows hides it, skip it; it is optional
4. Click **Commit changes**.
5. Go to **Settings → Pages**. Under *Build and deployment* set
   **Source: Deploy from a branch**, **Branch: main**, folder **/ (root)**. Save.
6. Wait ~1 minute. Your public link appears at the top of that page:

   `https://<your-username>.github.io/gk-quiz/`

---

## Option B — command line (keeps the git history)

Create the empty repo as in step 1 above, then in **Git Bash** (or GitHub
Desktop's terminal) inside `AM Preparation\gk-quiz-site`:

```bash
git remote add origin https://github.com/<your-username>/gk-quiz.git
git push -u origin main
```

Then do step 5 above (Settings → Pages → main → / (root)).

Windows will prompt you to sign in to GitHub the first time; after that it is
remembered.

---

## Updating it later

When more sessions are extracted, replace `index.html` and `question_bank.json`
and either re-upload them, or:

```bash
git add -A && git commit -m "add more sessions" && git push
```

Pages redeploys automatically within a minute.

---

## One thing worth deciding before you make it public

The questions and explanations come from Aashman Upadhaya's **GK For All** live
classes. The README and the page footer both credit the channel and link every
question back to the exact timestamp in the source video, which is the right way
to do it — but a public site is different from private study notes. It is worth
sending the channel a quick message to say you have built this and to ask
whether they are happy for it to be public. Most teachers say yes when they are
credited and linked; a few would rather it stayed private, and it is much easier
to ask first than to take it down later.

If you would rather keep it private for now, GitHub private repos do not serve
Pages on the free plan — but the single `index.html` works perfectly from your
own disk, or from any private host.
