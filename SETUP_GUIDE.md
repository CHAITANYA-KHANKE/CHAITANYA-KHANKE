# GitHub Profile Setup Guide

Aapke GitHub profile ko attractive aur dynamic banane ke liye, humne workspace me zaroori files create kar di hain:
1. `README.md` - Aapke details, badges, stats aur animations ka template.
2. `banner.svg` - Custom cyberpunk designer banner.
3. `.github/workflows/profile-animations.yml` - Space Shooter aur Snake games auto-generate karne ka workflow.

Aapko in files ko apne GitHub par upload karna hoga. Neeche diye gaye steps ko follow karein:

---

### Step 1: GitHub par "Special" Repository banayein
1. Apne GitHub account par jayein aur ek new repository create karein.
2. Repository name exactly aapka username hona chahiye: **`CHAITANYA-KHANKE`**.
3. **MANDATORY:** Ise **Public** select karein.
4. **Initialize this repository with** checkbox me kisi bhi cheez ko tick *mat* karein (na README, na gitignore). Ekdam empty repo banayein.

---

### Step 2: Apne Local Files ko Push karein
Apne terminal ya VS Code internal terminal me ye commands run karein:

```bash
# 1. Workspace folder me jayein
cd "c:\Users\chait\Documents\RESEARCH"

# 2. Git initialize karein
git init -b main

# 3. Remote origin set karein (apna github url dalein)
git remote add origin https://github.com/CHAITANYA-KHANKE/CHAITANYA-KHANKE.git

# 4. Files add karein
git add README.md banner.svg .github/

# 5. Commit karein
git commit -m "Initial commit: Professional profile README & workflow"

# 6. Push karein main branch par
git push -u origin main
```

---

### Step 3: GitHub Actions Workflow ko run karein
Aapka contribution game generate hone ke liye, GitHub Action ko pehli baar chalana padega:
1. Apne GitHub repository (**`CHAITANYA-KHANKE/CHAITANYA-KHANKE`**) par jayein.
2. **Actions** tab par click karein.
3. Left sidebar me **"Generate Profile Animations"** select karein.
4. **"Run workflow"** dropdown par click karke, fir se **"Run workflow"** button par click karein.
5. 1-2 minutes wait karein. Workflow successful hone ke baad, ye automatic ek new branch `output` banayega aur usme `game.gif` aur `github-contribution-grid-snake.svg` push kar dega.

**Congratulation!** Jaise hi workflow complete hoga, aapki profile README refresh karne par Space Shooter aur Snake game dikhne lagenge.
