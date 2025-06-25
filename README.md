# GitHub Pages Setup for Legal Documents

## 🚀 Quick Setup Guide

### Step 1: Create GitHub Repository
1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right → "New repository"
3. Name it: `guided-legal`
4. Make it **Public** (required for free GitHub Pages)
5. Click "Create repository"

### Step 2: Upload Legal Documents
1. In your new repository, click "uploading an existing file"
2. Drag and drop these files:
   - `terms-of-use.html`
   - `privacy-policy.html`
   - `README.md` (this file)
3. Click "Commit changes"

### Step 3: Enable GitHub Pages
1. Go to your repository **Settings** tab
2. Scroll down to "Pages" section (left sidebar)
3. Under "Source", select "Deploy from a branch"
4. Choose "main" branch and "/ (root)" folder
5. Click "Save"

### Step 4: Get Your URLs
Your legal documents will be available at:
- **Terms of Use**: `https://[your-username].github.io/guided-legal/terms-of-use.html`
- **Privacy Policy**: `https://[your-username].github.io/guided-legal/privacy-policy.html`

Replace `[your-username]` with your actual GitHub username.

## 🔧 Update Your App

Once you have your URLs, update them in `PaywallScreen.js`:

```javascript
const openTermsOfUse = () => {
  Linking.openURL('https://[your-username].github.io/guided-legal/terms-of-use.html');
};

const openPrivacyPolicy = () => {
  Linking.openURL('https://[your-username].github.io/guided-legal/privacy-policy.html');
};
```

## 📋 App Store Connect Updates

### Privacy Policy Field
Add your Privacy Policy URL:
```
https://[your-username].github.io/guided-legal/privacy-policy.html
```

### App Description Addition
Add this to your App Store description:
```
Terms of Use: https://[your-username].github.io/guided-legal/terms-of-use.html
```

## ✅ Verification Checklist

- [ ] Repository created and public
- [ ] Legal documents uploaded
- [ ] GitHub Pages enabled
- [ ] URLs working (test in browser)
- [ ] App updated with correct URLs
- [ ] App Store Connect updated
- [ ] New app build created and tested

## 🎯 Next Steps

1. **Test the links** in your app
2. **Build a new version** of your app
3. **Submit to App Store Connect**
4. **Include the URLs** in your submission notes

Your app should now pass the App Store review! 🎉 