# GitHub Pages Deployment Guide

This guide will walk you through deploying your portfolio website to GitHub Pages at `fontzgui.github.io`.

## Prerequisites

- [x] GitHub account: `fontzgui`
- [x] Repository created: `fontzgui.github.io`
- [x] Git installed on your machine
- [x] Portfolio files ready in `/portfolio-site/` directory

## Step-by-Step Deployment

### 1. Navigate to Portfolio Directory

```bash
cd /Users/fontzg/code/anthropic/jobhunterproai/new_version_folder/portfolio-site
```

### 2. Initialize Git Repository (if not already done)

```bash
# Initialize git
git init

# Add remote (replace with your actual repo URL)
git remote add origin https://github.com/fontzgui/fontzgui.github.io.git
```

### 3. Add All Files

```bash
# Add all files to staging
git add .

# Check what will be committed
git status
```

You should see:
- `index.html`
- `project.html`
- `about.html`
- `contact.html`
- `README.md`
- `DEPLOYMENT_GUIDE.md` (this file)

### 4. Create Initial Commit

```bash
git commit -m "Initial portfolio deployment: AI-first development showcase

- Homepage with 5-step AI-assisted development framework
- DreamVelo case study (28 STRIDE threats, zero incidents)
- About page (AI Security + Product Engineer)
- Contact page (guillfontz@gmail.com, LinkedIn)
- README with key metrics and technology stack"
```

### 5. Push to GitHub

```bash
# Push to main branch
git push -u origin main
```

If you get an error about the branch name, you might need to rename it:

```bash
# Rename branch to main if needed
git branch -M main
git push -u origin main
```

### 6. Configure GitHub Pages

1. Go to your repository: https://github.com/fontzgui/fontzgui.github.io
2. Click **Settings** (top right)
3. Scroll down to **Pages** section (left sidebar under "Code and automation")
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

### 7. Wait for Deployment (1-2 minutes)

GitHub will automatically build and deploy your site. You'll see:
- ✅ Green checkmark when ready
- 🔗 Your site URL: `https://fontzgui.github.io`

### 8. Verify Deployment

Visit https://fontzgui.github.io and verify:
- [x] Homepage loads with AI-first development messaging
- [x] Navigation works (all 4 pages accessible)
- [x] Contact links work (email: guillfontz@gmail.com, LinkedIn)
- [x] Mobile responsive (test on phone/tablet)
- [x] No console errors (F12 → Console tab)

## Making Updates Later

When you want to update your portfolio:

```bash
# 1. Make your changes to HTML files
# 2. Add and commit
git add .
git commit -m "Update: [describe your changes]"

# 3. Push to GitHub
git push

# 4. Wait 1-2 minutes for GitHub Pages to rebuild
```

## Common Issues & Fixes

### Issue: "Permission denied (publickey)"

**Fix:** You need to authenticate with GitHub. Either:

**Option A: HTTPS (easier)**
```bash
# Use HTTPS URL instead of SSH
git remote set-url origin https://github.com/fontzgui/fontzgui.github.io.git
git push
# Enter GitHub username and personal access token when prompted
```

**Option B: SSH (recommended long-term)**
```bash
# Generate SSH key
ssh-keygen -t ed25519 -C "guillfontz@gmail.com"

# Add to SSH agent
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519

# Copy public key
cat ~/.ssh/id_ed25519.pub
# Add this key to GitHub: Settings > SSH and GPG keys > New SSH key
```

### Issue: 404 Error After Deployment

**Fix:**
1. Ensure `index.html` exists in root directory
2. Check GitHub Pages settings (Settings > Pages)
3. Wait 5 minutes for DNS propagation
4. Clear browser cache (Cmd+Shift+R on Mac)

### Issue: CSS Not Loading (Tailwind)

**Fix:**
- Tailwind is loaded from CDN, so no build process needed
- Check if you have internet connection
- Verify CDN URL: `https://cdn.tailwindcss.com`

### Issue: Contact Form Not Working

**Note:** The contact form currently shows a success message without actually sending email. To implement real email sending:

1. Sign up for FormSpree: https://formspree.io
2. Create a form, get your form ID
3. Update `contact.html` line 324 with your form ID
4. Uncomment lines 322-346 in `contact.html`
5. Comment out lines 301-319 (simulation code)

## Custom Domain (Optional)

If you want to use a custom domain like `guillaumefontz.com`:

1. Buy domain from Namecheap/GoDaddy/Cloudflare
2. Add `CNAME` file to repository root:
   ```
   guillaumefontz.com
   ```
3. Configure DNS at your domain provider:
   ```
   Type: CNAME
   Name: @
   Value: fontzgui.github.io
   ```
4. Update GitHub Pages settings with custom domain
5. Enable HTTPS (GitHub provides free SSL certificate)

## Next Steps After Deployment

1. **Test thoroughly:**
   - Desktop browsers (Chrome, Firefox, Safari)
   - Mobile devices (iOS, Android)
   - Check all navigation links
   - Verify contact links work

2. **Update LinkedIn:**
   - Add portfolio URL to profile
   - Update headline to reflect AI-first development focus
   - Share portfolio in a post

3. **Share with network:**
   - Email to recruiters/contacts
   - Post on Twitter/X
   - Add to resume

4. **Monitor:**
   - Set up Google Analytics (optional)
   - Track which pages get most views
   - Update based on feedback

## Files You Can Safely Modify

**HTML Files:**
- `index.html` - Homepage content
- `project.html` - DreamVelo case study details
- `about.html` - Your background and skills
- `contact.html` - Contact information

**Documentation:**
- `README.md` - Repository documentation
- `DEPLOYMENT_GUIDE.md` - This file

**DO NOT modify:**
- Git configuration files (`.git/` directory)

## Support

If you encounter issues:
1. Check GitHub Pages documentation: https://docs.github.com/en/pages
2. Verify GitHub Pages status: https://www.githubstatus.com
3. Review commit history: `git log`
4. Check deployment logs in GitHub Actions tab

## Maintenance

**Recommended updates:**
- Update metrics as DreamVelo grows (user count, MRR, etc.)
- Add new projects/case studies as you build them
- Keep technology stack current
- Refresh screenshots if you redesign DreamVelo

---

**Ready to deploy?** Run the commands in Step 1-5 above!

After deployment, your portfolio will be live at: **https://fontzgui.github.io**
