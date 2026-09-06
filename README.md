# समसामयिक Quiz — Daily GK practice

A single-page, offline-capable practice quiz built from the **GK For All — Daily GK
live exam** sessions by **Aashman Upadhaya**.

**Live:** https://USERNAME.github.io/REPO/

## How it works

- **सबै प्रश्न — Start** runs the whole bank.
- **Random 20** gives a quick mixed set.
- **Pick dates** lets you practise one session, or several, at a time.

Questions and answer options are shuffled on every run. After each answer you get
the correct option, a short explanation, and a deep link to the exact moment in
the source video.

Your score history is kept in your own browser (localStorage). Nothing is uploaded.

## Where the content comes from

Every question was read off the screen of the original livestreams — the on-screen
poll result boards (each prints its own question number) and, where no poll was
run, the instructor's own marking on the blackboard. Answers are recorded as the
source presents them. Where a source answer differs from the internationally
accepted fact, the explanation says so rather than silently "correcting" it.

All credit for the teaching content belongs to the original channel. This is a
study aid, not a replacement — please watch the sessions.

## Files

| file | what it is |
|---|---|
| `index.html` | the quiz — everything is embedded, works offline |
| `question_bank.json` | the raw question data |
| `extraction_tracker.html` | which sessions have been processed |
| `extracted_content.html` | searchable date-wise revision sheet |
