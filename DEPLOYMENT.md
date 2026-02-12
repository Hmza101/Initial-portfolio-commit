# Deploying Your Portfolio Online

## Option 1: GitHub Pages (Free & Recommended)

### Step 1: Create GitHub Repository
```bash
# Navigate to your portfolio folder
cd /home/hamza/my-servants/ai-agents/portfolio

# Initialize Git repository
git init
git add .
git commit -m "Initial portfolio commit"

# Create GitHub repository at: https://github.com/new
# Then push to GitHub:
git remote add origin https://github.com/yourusername/your-repo-name.git
git branch -M main
git push -u origin main
```

### Step 2: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click Settings → Pages
3. Source: "Deploy from a branch"
4. Branch: "main" and "/ (root)"
5. Click Save
6. Your site will be live at: `https://yourusername.github.io/your-repo-name`

---

## Option 2: Netlify (Free & Easy)

### Method A: Drag & Drop
1. Go to [netlify.com](https://netlify.com)
2. Sign up for free
3. Drag your entire `portfolio` folder onto the "Deploy area"
4. Your site is instantly live with a random URL

### Method B: GitHub Integration
1. Push to GitHub (as above)
2. Connect Netlify to your GitHub account
3. Select your repository
4. Deploy settings auto-detect your static site
5. Your site is live with automatic deployments

---

## Option 3: Vercel (Free & Modern)

### Method A: CLI
```bash
# Install Vercel CLI
npm i -g vercel

# Navigate to portfolio folder
cd /home/hamza/my-servants/ai-agents/portfolio

# Deploy
vercel --prod
```

### Method B: Website
1. Go to [vercel.com](https://vercel.com)
2. Import your Git repository
3. Vercel auto-detects it's a static site
4. Deploy with one click

---

## Option 4: Firebase Hosting (Free)

```bash
# Install Firebase CLI
npm install -g firebase-tools

# Navigate to portfolio folder
cd /home/hamza/my-servants/ai-agents/portfolio

# Initialize Firebase
firebase init hosting
# Follow prompts:
# - Use existing project or create new
# - Public directory: .
# - Configure as single-page app: No
# - Overwrite index.html: No

# Deploy
firebase deploy
```

---

## Option 5: GitHub Pages with Custom Domain

### For custom domain like `yourname.com`:
1. Deploy with GitHub Pages (Option 1)
2. In repo Settings → Pages → Custom domain
3. Add your domain name
4. Configure DNS records with your domain provider

---

## Quick Deployment Checklist

### Before Deploying:
- [ ] Test portfolio locally by opening `index.html`
- [ ] Add your PDF resume as `CV.pdf`
- [ ] Update contact information if needed
- [ ] Check all links and images

### Portfolio URL Structure:
- GitHub Pages: `https://username.github.io/repo-name`
- Netlify: `https://random-name.netlify.app`
- Vercel: `https://your-project.vercel.app`
- Firebase: `https://your-project.web.app`

---

## Recommended: Netlify (Easiest)

**Netlify is recommended because:**
- No Git required (drag & drop)
- Instant deployment
- Free custom domain support
- Automatic HTTPS
- Form handling built-in
- No configuration needed

**Steps:**
1. Go to [netlify.com](https://netlify.com)
2. Drag your `portfolio` folder to the deploy area
3. Done! Your portfolio is live instantly.

---

## Pro Tips

### Custom Domain Setup:
- Purchase domain from Namecheap, GoDaddy, etc.
- Point DNS to your hosting provider
- Most providers offer free custom domains

### Portfolio Optimization:
- Compress images before uploading
- Enable HTTPS (most providers do this automatically)
- Set up analytics with Google Analytics
- Consider adding a contact form backend

### Update Process:
- GitHub Pages: Push changes to trigger redeploy
- Netlify: Drag & drop new files or connect Git
- Vercel: Push to Git or use CLI to redeploy

Need help with any specific deployment method?