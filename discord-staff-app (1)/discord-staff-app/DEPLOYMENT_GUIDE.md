# Complete Deployment Guide - GitHub to Vercel

## Step 1: Prepare Your GitHub Account

### If you don't have GitHub yet:
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Follow the signup process
4. Verify your email

### If you already have GitHub:
- Just login to your account

---

## Step 2: Create a New Repository on GitHub

1. Go to [github.com/new](https://github.com/new)
2. Enter repository name: `discord-staff-app` (or your preferred name)
3. Description (optional): "Discord Staff Application System"
4. Choose **Public** (so it can be deployed)
5. ✅ Check "Add a README file"
6. Click **"Create repository"**

---

## Step 3: Upload Files to GitHub

### Option A: Using GitHub's Web Interface (Easiest)

1. On your new repository page, click **"Add file"** → **"Upload files"**
2. Drag and drop these files into the upload area:
   - `index.html`
   - `package.json`
   - `vercel.json`
   - `.gitignore`
   - `README.md`
   - `DEPLOYMENT_GUIDE.md`

3. Add commit message: `Initial commit - Discord Staff Application`
4. Click **"Commit changes"**

### Option B: Using Git Command Line (Recommended)

1. Install Git from [git-scm.com](https://git-scm.com)
2. Open terminal/command prompt
3. Navigate to your project folder:
   ```bash
   cd path/to/discord-staff-app
   ```

4. Initialize Git and upload:
   ```bash
   git init
   git add .
   git commit -m "Initial commit - Discord Staff Application"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/discord-staff-app.git
   git push -u origin main
   ```
   
   ⚠️ Replace `YOUR_USERNAME` with your actual GitHub username!

5. If prompted for credentials:
   - Enter your GitHub username
   - For password, use a **Personal Access Token** (not your password):
     - Go to GitHub Settings → Developer settings → Personal access tokens
     - Generate new token with `repo` scope
     - Copy and paste the token as password

---

## Step 4: Deploy to Vercel

### Connect Vercel to GitHub

1. Go to [vercel.com](https://vercel.com)
2. Click **"Sign Up"** or **"Log In"**
3. Choose **"Continue with GitHub"**
4. Authorize Vercel to access your GitHub account
5. Click **"Allow"**

### Deploy Your Repository

1. After connecting, Vercel will show your repositories
2. Find `discord-staff-app` in the list
3. Click **"Import"**
4. Click **"Deploy"**

### That's it! 🎉

Vercel will:
- Detect your project
- Build it
- Deploy it to a live URL
- Automatically redeploy on every GitHub push

Your site will be live at a URL like: `https://discord-staff-app.vercel.app`

---

## Step 5: Get Your Live Application Link

After deployment, you'll see:
- ✅ Deployment successful
- 📍 Live URL (e.g., `https://discord-staff-app.vercel.app`)

### Share this link with:
- **Applicants**: `https://your-domain.vercel.app` (click "Apply Now")
- **Staff**: `https://your-domain.vercel.app` (click "Admin Panel")

---

## Step 6: Make Changes Later

### Update Your Application

1. Edit files locally (e.g., change the scenario question)
2. Commit and push to GitHub:
   ```bash
   git add .
   git commit -m "Update: Changed moderation scenario"
   git push
   ```

3. Vercel automatically detects the push
4. Redeploys your site within seconds
5. No extra steps needed!

---

## Custom Domain (Optional)

### Connect Your Own Domain

1. Go to your Vercel project page
2. Click **"Settings"**
3. Go to **"Domains"**
4. Enter your domain name
5. Follow the DNS instructions provided by Vercel
6. Update DNS records at your domain provider
7. Wait for DNS to propagate (up to 48 hours)

---

## Troubleshooting Deployment

### Issue: "Failed to deploy"

**Solution:**
- Check all files are in repository
- Ensure `index.html` is in root directory
- Check GitHub is public repository
- Try redeploying from Vercel dashboard

### Issue: "Cannot import from Vercel"

**Solution:**
- Disconnect/reconnect GitHub at vercel.com/account/integrations
- Try creating new project from dashboard

### Issue: "Vercel won't find my repository"

**Solution:**
- Push files to GitHub first
- Wait 30 seconds for GitHub to sync
- Refresh Vercel page
- Check repository is set to Public

### Issue: "Site shows blank page"

**Solution:**
- Check browser console for errors (F12)
- Clear browser cache (Ctrl+Shift+Delete)
- Hard refresh (Ctrl+Shift+R)
- Check internet connection

---

## Environment Variables (If Needed Later)

If you add features requiring environment variables:

1. Go to Vercel Project **Settings**
2. Click **"Environment Variables"**
3. Add your variables
4. Redeploy

---

## Monitoring Your Deployment

### View Deployment Status

1. Go to [vercel.com/dashboard](https://vercel.com/dashboard)
2. Click your project
3. See real-time deployment status
4. View logs of any issues

### Enable Auto-Deployments

✅ This is enabled by default when connected to GitHub!

Every time you push to main branch:
- Vercel automatically redeploys
- No manual steps needed
- Live updates within 1-2 minutes

---

## Security Notes

⚠️ **Important:**
- This application stores data in browser's localStorage
- Data is NOT sent to any server
- Each user's browser has separate data
- Admin panel works from the same browser
- For production: Consider adding backend database

---

## Next Steps

1. ✅ Test the application
2. ✅ Try submitting a test application
3. ✅ Check admin panel
4. ✅ Share link with your Discord community
5. ✅ Monitor applications in admin panel

---

## Support

- **Vercel Docs**: https://vercel.com/docs
- **GitHub Help**: https://docs.github.com
- **Git Tutorial**: https://git-scm.com/book/en/v2

---

**Deployment Complete! Your Discord Staff Application is now live! 🚀**
