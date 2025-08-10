# Deployment Guide for Elshain Website

This guide will walk you through deploying your website to GitHub Pages with a custom domain (elshain.com).

## Prerequisites

1. **GitHub Account**: You need a GitHub account
2. **Domain Ownership**: You must own elshain.com
3. **Git**: Git should be installed on your computer

## Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Repository name: `elshain.github.io` (this is crucial for GitHub Pages)
5. Make it **Public** (required for free GitHub Pages)
6. Don't initialize with README (we already have one)
7. Click "Create repository"

## Step 2: Upload Your Website Files

### Option A: Using Git (Recommended)

1. **Initialize Git in your local folder**:
   ```bash
   cd /path/to/your/elshain/folder
   git init
   git add .
   git commit -m "Initial website setup"
   ```

2. **Connect to GitHub repository**:
   ```bash
   git remote add origin https://github.com/elshain/elshain.github.io.git
   git branch -M main
   git push -u origin main
   ```

### Option B: Using GitHub Web Interface

1. Go to your new repository on GitHub
2. Click "uploading an existing file"
3. Drag and drop all your website files
4. Add commit message: "Initial website setup"
5. Click "Commit changes"

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" section (in the left sidebar)
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

## Step 4: Configure Custom Domain

1. In the same Pages settings section
2. Under "Custom domain", enter: `elshain.com`
3. Check "Enforce HTTPS" (recommended)
4. Click "Save"

**Note**: It may take a few minutes for the domain to be verified.

## Step 5: Configure DNS Records

You need to configure your domain's DNS settings at your domain registrar (where you bought elshain.com).

### Add these DNS records:

#### A Records (for root domain):
```
Type: A
Name: @
Value: 185.199.108.153
TTL: 3600

Type: A
Name: @
Value: 185.199.109.153
TTL: 3600

Type: A
Name: @
Value: 185.199.110.153
TTL: 3600

Type: A
Name: @
Value: 185.199.111.153
TTL: 3600
```

#### CNAME Record (for www subdomain):
```
Type: CNAME
Name: www
Value: elshain.github.io
TTL: 3600
```

### Popular Domain Registrars:

**Namecheap**:
1. Go to Domain List → Manage
2. Click "Advanced DNS"
3. Add the records above

**GoDaddy**:
1. Go to My Products → DNS
2. Click "Manage DNS"
3. Add the records above

**Google Domains**:
1. Go to your domain → DNS
2. Click "Manage custom records"
3. Add the records above

## Step 6: Verify Setup

1. **Wait for DNS propagation** (can take up to 48 hours, usually much faster)
2. **Test your website**:
   - Visit `https://elshain.com`
   - Visit `https://www.elshain.com`
   - Both should show your website

3. **Check GitHub Pages status**:
   - Go to repository Settings → Pages
   - You should see a green checkmark
   - The custom domain should be listed

## Step 7: Test Everything

1. **Test responsive design** on different devices
2. **Test all links** and navigation
3. **Test contact form** (currently shows alert, you'll need backend for real functionality)
4. **Test loading speed** using tools like Google PageSpeed Insights

## Troubleshooting

### Website not loading:
- Check DNS propagation: https://www.whatsmydns.net/
- Verify DNS records are correct
- Wait up to 48 hours for full propagation

### HTTPS not working:
- Make sure "Enforce HTTPS" is checked in GitHub Pages settings
- Wait for SSL certificate to be issued (can take up to 24 hours)

### Custom domain not working:
- Verify the CNAME file contains `elshain.com`
- Check that the domain is entered correctly in GitHub Pages settings
- Ensure DNS records are properly configured

### 404 errors:
- Make sure your main file is named `index.html`
- Check that all file paths are correct
- Verify the repository is public

## Next Steps

1. **Customize content**: Update the website with your actual content
2. **Add images**: Replace placeholder images with your own
3. **Set up analytics**: Add Google Analytics or similar
4. **Add contact form backend**: Implement real form submission
5. **Optimize SEO**: Add more meta tags and structured data
6. **Add blog**: Consider adding a blog section using Jekyll

## Support

If you encounter issues:
1. Check GitHub Pages documentation: https://pages.github.com/
2. Verify DNS settings with your domain registrar
3. Check GitHub Pages status: https://www.githubstatus.com/

## Security Notes

- Keep your repository public (required for free GitHub Pages)
- Don't commit sensitive information like API keys
- Use environment variables for any sensitive data
- Regularly update dependencies if you add any

Your website should now be live at `https://elshain.com`! 🎉 