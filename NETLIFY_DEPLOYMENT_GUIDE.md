# Deploy Your Portfolio to Netlify (FREE) - Complete Guide

## What is Netlify?
- ✅ FREE hosting for static websites
- ✅ Automatic HTTPS/SSL
- ✅ Custom domain support (rijultandon.engineer)
- ✅ Fast CDN globally
- ✅ No credit card needed
- ✅ Perfect for portfolios

## STEP-BY-STEP DEPLOYMENT

### STEP 1: Install Git (if not already installed)
1. Download from: https://git-scm.com/download/win
2. Run installer with default settings
3. Restart your computer

### STEP 2: Prepare Your Project for Git
Open PowerShell in your website folder and run:

```powershell
cd c:\Users\letsc\Desktop\Details\website

# Initialize git
git init

# Add all files
git add .

# Make first commit
git commit -m "Initial portfolio commit"
```

### STEP 3: Create GitHub Account (if you don't have one)
1. Go to https://github.com/signup
2. Sign up with any email (suggest letscomerijul@gmail.com)
3. Verify email
4. Create a new repository:
   - Name: `portfolio` (or any name)
   - Description: "Rijul Tandon - Professional Portfolio"
   - Public
   - DO NOT initialize with README (your files already exist)
   - Click "Create repository"

### STEP 4: Push Your Project to GitHub
After creating the repo, GitHub shows commands. Run these in PowerShell:

```powershell
cd c:\Users\letsc\Desktop\Details\website

# Add GitHub remote
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git

# Rename branch to main
git branch -M main

# Push your files
git push -u origin main
```

**Replace YOUR_USERNAME with your actual GitHub username**

### STEP 5: Connect GitHub to Netlify
1. Go to https://netlify.com
2. Click "Sign up" (use your GitHub account)
3. Click "Connect with GitHub"
4. Authorize Netlify to access your GitHub
5. Click "Import an existing project"
6. Select your GitHub repository (`portfolio`)
7. Click "Deploy site"

**Netlify will automatically deploy!** ⚡

### STEP 6: Add Your Custom Domain
1. In Netlify dashboard for your site
2. Go to "Site settings" → "Domain management"
3. Click "Add custom domain"
4. Enter: `rijultandon.engineer`
5. Netlify will show DNS settings
6. Follow the steps to update Name.com DNS

#### Update DNS on Name.com:
1. Go to https://www.name.com (log in)
2. Find your domain: rijultandon.engineer
3. Click on it
4. Go to "DNS" section
5. You'll see Netlify's nameservers:
   - dns1.p01.nsone.net
   - dns2.p02.nsone.net
   - dns3.p03.nsone.net
   - dns4.p04.nsone.net
6. Copy these into Name.com's nameserver fields
7. Save changes
8. Wait 24-48 hours for DNS to update

### STEP 7: Enable HTTPS
1. Back in Netlify dashboard
2. Go to "Site settings" → "SSL/TLS certificate"
3. It should automatically provision (usually takes 5-10 minutes)
4. Once it shows "Active", HTTPS is enabled

### STEP 8: Verify Your Site
1. Wait 2-5 minutes for DNS propagation
2. Visit: https://rijultandon.engineer
3. Check:
   - ✅ Site loads correctly
   - ✅ HTTPS shows secure lock
   - ✅ Resume button downloads PDF
   - ✅ Smooth scrolling works
   - ✅ Mobile responsive

---

## QUICK REFERENCE COMMANDS

```powershell
# Navigate to folder
cd c:\Users\letsc\Desktop\Details\website

# Check git status
git status

# View commit history
git log

# After making changes to site, update GitHub:
git add .
git commit -m "Update portfolio"
git push
```

*When you push to GitHub, Netlify automatically redeploys your site!*

---

## COMMON ISSUES & FIXES

| Problem | Solution |
|---------|----------|
| Git not found | Restart PowerShell/Computer after Git install |
| GitHub SSH error | Use HTTPS URL instead of SSH |
| DNS not updating | Can take up to 48 hours, check later |
| Site shows 404 | Ensure index.html is in root of repo |
| CV won't download | Check RIJUL_CV.pdf is in same folder |
| HTTPS not working | Wait 10 minutes, refresh browser cache |

---

## UPDATING YOUR SITE IN THE FUTURE

Whenever you want to update your portfolio:

```powershell
cd c:\Users\letsc\Desktop\Details\website

# Edit your files (index.html, etc.)
# Then:

git add .
git commit -m "Update: Add new projects"
git push

# Netlify automatically deploys! (takes 30 seconds - 2 minutes)
```

---

## SUPPORT

- **Netlify Docs**: https://docs.netlify.com
- **GitHub Help**: https://docs.github.com
- **Name.com Support**: Contact them directly

---

## Summary

1. ✅ Install Git
2. ✅ Run git commands to initialize repo
3. ✅ Create GitHub account
4. ✅ Push to GitHub
5. ✅ Sign up on Netlify with GitHub
6. ✅ Connect your repository
7. ✅ Add custom domain rijultandon.engineer
8. ✅ Update DNS on Name.com
9. ✅ Wait for DNS propagation
10. ✅ Visit https://rijultandon.engineer

**Total time: ~15 minutes setup + 24-48 hours for DNS propagation**

Once DNS updates, your site is live! 🎉

---

Need help with any step? Let me know!
