# Quick Start: Deploy Your Portfolio to GitHub Pages

## Step 1: Create Your GitHub Repository

1. Go to **https://github.com/new**
2. Repository name: **`yourusername.github.io`** (replace `yourusername` with your actual GitHub username)
3. Description: "Professional Portfolio"
4. Make sure to select **Public** (required for GitHub Pages with Free plan)
5. Click **Create repository**

## Step 2: Connect Your Local Repository to GitHub

In PowerShell, navigate to your portfolio directory and run:

```powershell
cd "C:\Users\user\Documents\dev\profile"

# Set your GitHub username
$githubUser = "yourusername"  # Change this!

# Add the remote
git remote add origin https://github.com/$githubUser/$githubUser.github.io.git

# Rename branch to main (if not already)
git branch -M main

# Push to GitHub
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Source", select:
   - **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **Save**

## Step 4: Wait for Deployment

GitHub will automatically deploy your site. You can check the progress:
1. Go to your repository
2. Look for the **Actions** tab to see deployment progress
3. Your site will be live at: **https://yourusername.github.io**

This typically takes 1-2 minutes. Refresh your browser and check!

## Making Updates

Every time you update your portfolio content:

```powershell
cd "C:\Users\user\Documents\dev\profile"

# Make your edits to content files...

# Commit and push
git add .
git commit -m "Update portfolio: [describe your changes]"
git push
```

Your changes will automatically deploy within a few minutes!

## Common Updates

### Update Your Name and Bio
Edit: `content/authors/me/_index.md`

### Add/Update Your Resume
1. Update or replace: `static/uploads/resume.pdf`
2. Test the link works from your site

### Update Your Profile Picture
1. Replace or add your image to: `assets/media/authors/me/avatar.jpg`
2. Update the filename in `content/authors/me/_index.md` if needed

### Add a New Side Project
Follow the guide in `PORTFOLIO_GUIDE.md` → "Side Projects" section

### Add a New Work Project
Follow the guide in `PORTFOLIO_GUIDE.md` → "Work Projects" section

## Troubleshooting

### Changes not showing up?
1. Wait 2-3 minutes for deployment
2. Hard refresh your browser: Ctrl+Shift+R (Windows)
3. Check GitHub Actions tab for errors

### Error deploying?
1. Go to your repository's **Actions** tab
2. Look at the failed workflow for error details
3. Common issues:
   - Typos in frontmatter YAML
   - Missing image files
   - Invalid Markdown syntax

### Want to use a custom domain?
1. After initial deployment, go to **Settings** → **Pages**
2. Under "Custom domain", enter your domain
3. Follow GitHub's DNS configuration instructions

## Next Steps

1. ✅ Create GitHub repository
2. ✅ Push local code to GitHub
3. ✅ Enable GitHub Pages
4. ✅ Verify site is live
5. ⏭️ **Update your portfolio content with real information**
6. ⏭️ Add project images
7. ⏭️ Customize colors and settings if desired

See `PORTFOLIO_GUIDE.md` for detailed content update instructions!

---

**Questions?**
- HugoBlox Docs: https://docs.hugoblox.com
- GitHub Pages Docs: https://docs.github.com/en/pages
