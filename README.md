# Our instrument

**Play it here:** <!-- Paste your GitHub Pages link here, e.g. https://idbcourses.github.io/ht26-a3-group-01/ -->

**Group:** <!-- Names of everyone in the group -->

<!-- One or two sentences: what kind of instrument is it, and what is it like to play? -->

## How to play

<!-- Which keys do what? Fill in the table, and add a row for every key or group of keys. -->

| Key | What it does |
| --- | ------------ |
|     |              |

<!-- Anything else a player needs to know: how to get started, combinations of keys, a good thing to try first. -->

---

## About this assignment

**A3.** The full brief, the due date and the assessment criteria are on Canvas.

Hand in on Canvas: a `.zip` of `main`, and the link to your live page in the submission comment. The link also goes at the top of this README.

### The files

| File         | What goes in it                                                                                                 |
| ------------ | --------------------------------------------------------------------------------------------------------------- |
| `script.js`  | All of your code: settings, state, the sound, `update()`, `use()`, the controls and `setup()`                   |
| `shape.js`   | Ready-made code for shapes on the page. Use `createShape()` and its methods; you don't need to change this file |
| `index.html` | The page. Loads Tone.js and `script.js`                                                                         |
| `style.css`  | How the page and the shapes look                                                                                |

`script.js` is split into sections with headings. Agree who works in which section, so you get fewer conflicts.

Allowed: vanilla JavaScript and Tone.js. Not allowed: other libraries, and CSS transitions or animations.

### Run it

1. Open `index.html`, then run **Live Preview: Show Preview (External Browser)** from the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`).
2. Open the browser's developer tools (`F12`, or `Cmd+Option+I` on a Mac) and click the **Console** tab.
3. You should see a pink circle in the middle of the page. Click on the page, then press `A`. You should see `Key down: a` and `Key up: a` in the console.

### The live page

Every time something is merged into `main`, GitHub publishes it at the link at the top of this README. It takes a minute or two. To find the link: on github.com, go to **Settings → Pages**.

---

## Working together

`main` is what you hand in and what you show at the showcase, so **`main` must always run**. Nobody works on `main` directly: every change goes on a branch, and comes back to `main` through a pull request.

### The steps, for every task

1. **Pull `main`.** Switch to `main` (click the branch name in the bottom-left corner of VS Code), then click **Sync Changes** (or **Pull**) in the Source Control panel.
2. **Make a branch** for one task. Click the branch name in the bottom-left corner → **Create new branch…**. Name it after the feature, not the person: `drone`, `octave-keys`, `echo-effect`.
3. **Commit and push** to your branch. Commit small and often. The first time, click **Publish Branch**. Keep the branch short: a day or two at most.
4. **Bring in the latest `main`** before you open the pull request. Switch to `main` and pull. Switch back to your branch, then run **Git: Merge Branch…** from the Command Palette and choose `main`. If there's a conflict, see below. Run your code to check it still works, then push.
5. **Open a pull request** on github.com (GitHub shows a **Compare & pull request** button after you push). Fill in the three sections: _What changed_, _How to test it_, _Anything you're unsure about_, so your groupmates know what's coming into `main`.
6. **Merge it**: **Merge pull request** on github.com. Then click **Delete branch**.

Spread the work: everyone writes code, and each of you should open pull requests.

### When you get a conflict

A conflict means two branches changed the same lines, and Git can't tell which version to keep. It's normal, and nothing is lost. You decide.

1. The Source Control panel lists the conflicting files under **Merge Changes**. Open one.
2. Each conflict shows two versions: **Current** (your branch) and **Incoming** (`main`). Above each one, click **Accept Current Change**, **Accept Incoming Change** or **Accept Both Changes**. Or edit the lines by hand until they're right.
3. Make sure no `<<<<<<<`, `=======` or `>>>>>>>` lines are left in the file.
4. Save, then click **+** next to the file to stage it.
5. When every file is done, click **Commit**, then push.
6. **Run the code.** A conflict you've resolved can still break the program.

To have fewer conflicts: pull `main` often, keep branches short, and agree who works in which file. Two people working on the same function at the same time will get a conflict.

If you're stuck, stop and ask a TA or teacher. Don't delete the folder and clone again, and don't force anything.
