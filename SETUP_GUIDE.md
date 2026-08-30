# 🚀 GitHub Pages Setup Guide
## ForecastIQ ko GitHub pe live karne ke exact steps

---

## Step 1 — GitHub Account & New Repo banao

1. GitHub.com pe login karein
2. Top-right corner mein **"+"** icon → **"New repository"** click karein
3. Fill karein:
   - **Repository name:** `forecastiq`
   - **Description:** `Sales Intelligence & Forecasting Platform`
   - **Visibility:** ✅ Public  ← (GitHub Pages free mein sirf Public repo pe kaam karta hai)
   - **Add README:** ❌ Uncheck (hum apna README upload karenge)
4. **"Create repository"** click karein

---

## Step 2 — Files Upload karein (No coding needed!)

GitHub pe jaake **"uploading an existing file"** link click karein, ya:

1. Repo page pe **"Add file"** → **"Upload files"** click karein
2. In files ko drag & drop karein:
   ```
   ✅ index.html          ← Main app (zaroor chahiye)
   ✅ README.md           ← Project description
   ✅ LICENSE             ← License file
   ✅ .gitignore          ← Optional
   ```
3. **Important:** `.github/workflows/deploy.yml` file bhi upload karein
   - Pehle `.github` folder banao → phir `workflows` folder → phir `deploy.yml` upload karein
   - Ya Git command se karo (Step 3 dekho)

4. Commit message: `Initial commit — ForecastIQ v1.0`
5. **"Commit changes"** click karein

---

## Step 3 — Git se upload karein (Recommended)

Agar Git installed hai:

```bash
# 1. Repo clone karein (YOUR_USERNAME replace karein)
git clone https://github.com/YOUR_USERNAME/forecastiq.git
cd forecastiq

# 2. Files copy karein is folder mein
# (index.html, README.md, LICENSE, .gitignore, .github/ folder)

# 3. Push karein
git add .
git commit -m "Initial commit — ForecastIQ v1.0"
git push origin main
```

---

## Step 4 — GitHub Pages Enable karein

1. GitHub repo page pe **"Settings"** tab click karein
2. Left sidebar mein **"Pages"** click karein
3. **Source** section mein:
   - **"Deploy from a branch"** select karein
   - Branch: **`main`** (ya `master`)
   - Folder: **`/ (root)`**
4. **"Save"** click karein

> ⏱️ 2-3 minute wait karein. GitHub Pages automatically deploy hoga.

---

## Step 5 — (Optional) GitHub Actions se Auto-Deploy

Agar `.github/workflows/deploy.yml` file upload ki hai to:

1. Settings → Pages → Source → **"GitHub Actions"** select karein
2. Ab har baar push karne pe automatically deploy hoga!

---

## Step 6 — Live URL check karein

Deploy hone ke baad URL milega:
```
https://YOUR_USERNAME.github.io/forecastiq
```

Repo Settings → Pages mein dikhai dega:
```
✅ Your site is live at https://YOUR_USERNAME.github.io/forecastiq
```

---

## Step 7 — README mein URL update karein

`README.md` file mein `YOUR_USERNAME` ko apne actual GitHub username se replace karein:

```markdown
# Pehle (README.md mein)
[![Live Demo](https://img.shields.io/badge/...)](https://YOUR_USERNAME.github.io/forecastiq)

# Baad mein (apna username daalo)
[![Live Demo](https://img.shields.io/badge/...)](https://vikasmehra.github.io/forecastiq)
```

---

## ✅ Final Checklist

```
□ GitHub repo created (Public)
□ index.html uploaded
□ README.md uploaded  
□ LICENSE uploaded
□ .github/workflows/deploy.yml uploaded
□ GitHub Pages enabled (Settings → Pages → main branch)
□ Live URL working
□ README mein YOUR_USERNAME replace kiya
```

---

## 🔗 Share karne ke liye

Portfolio ya LinkedIn pe ye add karein:

```
🚀 ForecastIQ — Sales Intelligence & Forecasting Platform
Live Demo: https://YOUR_USERNAME.github.io/forecastiq
GitHub: https://github.com/YOUR_USERNAME/forecastiq

Features: 7 forecasting models (SARIMA, XGBoost, Ensemble),
scenario simulator, event calendar, executive reports — 
all in a single HTML file, no backend needed.
```

---

## ❓ Common Issues

**Problem:** Pages tab nahi dikh raha  
**Fix:** Repo Public hona chahiye. Settings → General → Change visibility → Public

**Problem:** 404 error aa raha hai  
**Fix:** Check karein ki file ka naam exactly `index.html` hai (lowercase)

**Problem:** Deploy hone mein time lag raha hai  
**Fix:** 3-5 minutes wait karein. GitHub Actions tab mein progress dekh sakte hain.

**Problem:** `.github` folder upload nahi ho raha  
**Fix:** GitHub web UI se hidden folders upload nahi hote. Git command line use karein.
