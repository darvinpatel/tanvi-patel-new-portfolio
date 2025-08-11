# 🚀 Netlify Deployment Guide

## Quick Deploy (Recommended)

### Method 1: Deploy from GitHub
1. Go to [netlify.com](https://netlify.com)
2. Sign up/Login with your GitHub account
3. Click **"New site from Git"**
4. Choose **GitHub** and select repository: `darvinpatel/tanvi-patel-new-portfolio`
5. **Build settings:**
   - **Build command**: `npm run build`
   - **Publish directory**: `.` (root directory)
6. Click **"Deploy site"**

### Method 2: Drag & Drop
1. Go to [netlify.com](https://netlify.com)
2. Drag your entire project folder to the deploy area
3. Netlify will automatically detect it's a static site

## 📁 Project Output Structure

Your project is already structured as a static website with the following output:

```
tanvi-new-portfolio/
├── index.html              # Main portfolio page
├── work.html               # Work showcase
├── contact.html            # Contact page
├── styles.css              # Main stylesheet
├── assets/                 # Images and media
│   ├── me.jpeg
│   ├── project1.jpeg
│   └── project1-img1.jpeg
├── qgis-project/           # Interactive map
│   ├── index.html          # Map page
│   ├── layers/             # Map data
│   ├── resources/          # Libraries
│   └── styles/             # Map styling
├── netlify.toml            # Netlify configuration
├── package.json            # Build configuration
└── README.md               # Project documentation
```

## ⚙️ Build Configuration

### netlify.toml
- **Publish directory**: `.` (current directory)
- **Build command**: `npm run build`
- **Security headers**: Configured for better security
- **Caching**: Optimized for static assets

### package.json
- **Build script**: `npm run build`
- **Dev server**: `npm run dev`
- **Deploy script**: `npm run deploy`

## 🔧 Advanced Deployment

### Using Netlify CLI
```bash
# Install Netlify CLI
npm install -g netlify-cli

# Login to Netlify
netlify login

# Deploy to Netlify
netlify deploy --prod --dir=.
```

### Environment Variables
If you need environment variables, add them in Netlify dashboard:
1. Go to Site settings > Environment variables
2. Add any required variables

## 🌐 Custom Domain
1. Go to Site settings > Domain management
2. Add your custom domain
3. Configure DNS settings as instructed

## 📊 Performance Features
- **Automatic HTTPS**: Enabled by default
- **Global CDN**: Fast loading worldwide
- **Asset optimization**: Automatic compression
- **Caching**: Optimized for static files

## 🔄 Continuous Deployment
- **Auto-deploy**: Every push to main branch
- **Preview deployments**: For pull requests
- **Rollback**: Easy version management

## 🛠️ Troubleshooting

### Build Issues
- Check build logs in Netlify dashboard
- Verify all files are committed to GitHub
- Ensure no large files (>100MB) are included

### QGIS Map Issues
- Large map files are excluded for deployment compatibility
- Consider hosting large files externally (CDN)
- Map will work with available smaller layers

## 📞 Support
- **Netlify Docs**: [docs.netlify.com](https://docs.netlify.com)
- **GitHub Issues**: [Repository Issues](https://github.com/darvinpatel/tanvi-patel-new-portfolio/issues)

## 🎯 Benefits of Netlify
- ✅ **Better file size limits** than Vercel
- ✅ **Git LFS support** for large files
- ✅ **Global CDN** for fast loading
- ✅ **Automatic HTTPS** and security
- ✅ **Easy rollbacks** and version control
- ✅ **Preview deployments** for testing
