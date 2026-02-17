# 🚀 GitHub Deployment Guide

## Option 1: GitHub CLI (Fastest)

If you have GitHub CLI installed:

```bash
cd restaurant-prompt-generator
gh auth login
gh repo create restaurant-prompt-generator --public --source=. --push
```

Then go to [vercel.com](https://vercel.com) and import the repository.

---

## Option 2: GitHub Desktop (Easiest for Non-Developers)

1. **Download GitHub Desktop**: https://desktop.github.com/
2. **Open GitHub Desktop** and sign in
3. **File → Add Local Repository**
4. **Select this folder**: `restaurant-prompt-generator`
5. **Publish Repository** (button in top right)
6. **Choose settings**:
   - Name: `restaurant-prompt-generator`
   - Make it Public ✓
7. **Click "Publish Repository"**
8. **Done!** Your code is on GitHub

### Deploy to Vercel:
1. Go to [vercel.com](https://vercel.com)
2. Click "Import Project"
3. Select your GitHub repository
4. Click "Deploy"
5. Live in 30 seconds! 🎉

---

## Option 3: Command Line (Traditional)

```bash
cd restaurant-prompt-generator

# Initialize git
git init

# Add all files
git add .

# First commit
git commit -m "Initial commit: Restaurant Midjourney Prompt Generator"

# Create repo on GitHub first, then:
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/restaurant-prompt-generator.git
git push -u origin main
```

Then deploy to Vercel as described above.

---

## Option 4: Drag & Drop to Vercel (No GitHub Needed)

1. Go to [vercel.com](https://vercel.com)
2. Click "Add New Project"
3. **Drag the entire folder** onto the page
4. Click "Deploy"
5. Done! (But won't have GitHub integration)

---

## After Deployment

### Your Live URLs:
- **Vercel**: `https://restaurant-prompt-generator.vercel.app`
- **GitHub**: `https://github.com/YOUR-USERNAME/restaurant-prompt-generator`

### Add Custom Domain (Optional):
1. Go to Vercel Dashboard → Your Project → Settings → Domains
2. Add your domain (e.g., `prompts.yourrestaurant.com`)
3. Follow DNS instructions
4. Done!

---

## Updating Your Site

### With GitHub:
```bash
# Make changes to index.html
git add .
git commit -m "Updated prompt options"
git push
```
Vercel auto-deploys on every push! 🚀

### Without GitHub:
Re-drag the folder to Vercel to update.

---

## Need Help?

- **GitHub Issues**: Problems with the code
- **Vercel Docs**: https://vercel.com/docs
- **GitHub Docs**: https://docs.github.com
