# Aathma Merin Bejoy — Bioinformatics Website 🧬

Your personal GitHub Pages site: a portfolio + a living learning roadmap from
biology/coding basics all the way to the 2026 frontier of AI in biology.

## What's inside

```
your-site/
├── index.html                 ← the main website (hero, about, roadmap, blog list, projects, links)
├── fasta-fastq-phred.html     ← your first blog post, styled to match
└── README.md                  ← this file
```

Everything sits in **one flat folder** — no subfolders — so uploading is as simple
as selecting all the files at once.

Everything is plain HTML/CSS — **no build step, no Jekyll needed**. Push it and it just works.

---

## 🚀 Publish it at aatsbioinfo.github.io (5 minutes)

Because your username is **AatsBioinfo**, GitHub gives you one special "user site"
at `https://AatsBioinfo.github.io`. Here's the exact recipe.

### Option A — all in the browser (easiest, no commands)

1. Go to **https://github.com/new** while signed in.
2. Repository name: type exactly **`AatsBioinfo.github.io`** (must match your username + `.github.io`).
3. Set it to **Public**, then click **Create repository**.
4. On the new empty repo page, click **“uploading an existing file”**.
5. Select **all the files** (`index.html`, `fasta-fastq-phred.html`, `README.md`) and drag them in — or use "choose your files" and multi-select them (hold ⌘ to pick more than one).
6. Scroll down, click **Commit changes**.
7. Wait ~1 minute, then open **https://AatsBioinfo.github.io** 🎉

That's it — GitHub Pages turns on automatically for a repo named `username.github.io`.

### Option B — with Git on your Mac (aathma-mac)

```bash
# 1. Create the repo on github.com first (name it AatsBioinfo.github.io), then:
cd ~/Desktop            # or wherever you unzipped this folder
git init
git add .
git commit -m "Launch my bioinformatics site"
git branch -M main
git remote add origin https://github.com/AatsBioinfo/AatsBioinfo.github.io.git
git push -u origin main
```

Then visit **https://AatsBioinfo.github.io** after a minute.

> If Pages doesn't appear, go to the repo → **Settings → Pages** and confirm
> the source is set to **Deploy from a branch → main → /(root)**.

---

## ✍️ Adding your next blog post

1. Copy `fasta-fastq-phred.html` to a new file, e.g. `fastqc-explained.html`.
2. Change the title, date, and body text inside it.
3. Open `index.html`, find the **BLOG** section, and turn one of the
   “Coming soon” cards into a real link:

```html
<a class="post" href="fastqc-explained.html">
  <div class="cover c2"><span class="mono">FastQC</span></div>
  <div class="post-body">
    <span class="date">Aug 2026 · 5 min read</span>
    <h3>What FastQC Is Really Telling You</h3>
    <p>Your short summary here…</p>
    <span class="read">Read post →</span>
  </div>
</a>
```

4. Commit/upload, and it's live.

---

## 🎨 Quick things you may want to change

| What | Where in `index.html` |
|------|------------------------|
| Your LinkedIn / Kaggle links | Search for `linkedin.com` and `kaggle.com` in the **CONNECT** section — paste your real profile URLs |
| Add your photo | Replace the DNA `<svg>` inside `.avatar` with `<img src="me.jpg" style="width:100%;height:100%;border-radius:50%;object-fit:cover">` (drop `me.jpg` in the folder) |
| Roadmap wording | Each `<div class="stage">` block is one step — edit the `<h3>`, `<p>`, and `<span class="tool">` chips |
| Mark a stage “done” | Change its `lvl-tag` text/colour, e.g. to `✓ Done` |
| Colours | Edit the `:root` variables at the top of the `<style>` block (`--coral`, `--violet`, `--teal`, …) |

---

## 🗺️ Your roadmap at a glance

0. **Foundations** — molecular biology, Linux/Bash, Git, Python, R
1. **Data & File Formats** — FASTA, FASTQ, Phred, SAM/BAM, VCF, GFF ← *you are here*
2. **Sequence Analysis** — QC, trimming, alignment, variant calling
3. **Genomics & Transcriptomics** — RNA-seq, assembly, single-cell
4. **Stats, Pipelines & Reproducibility** — statistics, Nextflow/Snakemake, Docker
5. **Machine Learning in Biology** — scikit-learn on omics data
6. **Deep Learning** — PyTorch, CNNs, transformers
7. **★ The 2026 Frontier** — ESM protein LMs, AlphaFold 3, Boltz-2, Evo 2, scGPT/Geneformer

Happy building — and welcome to learning in public! 🌱
