# 🚀 LUXE Theme - Quick Installation Guide

## Prerequisites
- Active Shopify store
- Admin access to your Shopify account
- Basic familiarity with Shopify admin

---

## Installation Method 1: ZIP Upload (Easiest - 5 minutes)

### Step 1: Prepare the Theme
1. Download the complete `shopify-luxe-theme` folder
2. Create a ZIP file of the entire folder:
   - **Windows**: Right-click folder → "Send to" → "Compressed (zipped) folder"
   - **Mac**: Right-click folder → "Compress"
   - **Linux**: `zip -r luxe-theme.zip shopify-luxe-theme/`

### Step 2: Upload to Shopify
1. Log into your Shopify Admin
2. Go to **Online Store** → **Themes**
3. Click **Add theme** → **Upload zip file**
4. Select your `luxe-theme.zip` file
5. Wait for upload to complete (30-60 seconds)

### Step 3: Publish Theme
1. Find "Luxe Fashion & Beauty" in your theme library
2. Click **Actions** → **Publish**
3. Confirm publication

**🎉 Done! Your theme is now live.**

---

## Installation Method 2: Shopify CLI (Developers - 10 minutes)

### Step 1: Install Shopify CLI
```bash
# Using npm
npm install -g @shopify/cli @shopify/theme

# Using Homebrew (Mac)
brew tap shopify/shopify
brew install shopify-cli

# Verify installation
shopify version
```

### Step 2: Navigate to Theme Directory
```bash
cd path/to/shopify-luxe-theme
```

### Step 3: Connect to Your Store
```bash
# Login to Shopify
shopify auth login

# Connect to your store
shopify theme dev --store your-store.myshopify.com
```

### Step 4: Preview & Push
```bash
# Preview locally (opens browser)
shopify theme dev

# Push to Shopify when ready
shopify theme push

# Or push and publish immediately
shopify theme push --publish
```

---

## Post-Installation Setup (10 minutes)

### 1. Configure Theme Settings
1. Go to **Online Store** → **Themes**
2. Click **Customize** on Luxe theme
3. Set your brand colors:
   - **Theme Settings** → **Colors**
   - Set primary, background, button colors

### 2. Upload Your Logo
1. In theme editor: **Header** section
2. Click **Select image** under Logo
3. Upload your logo (recommended: 200x60px PNG with transparency)

### 3. Set Up Navigation
1. **Online Store** → **Navigation**
2. Edit **Main menu**:
   - Add: Shop All, Fashion, Beauty, Accessories, Sale
   - Drag to reorder
3. Save changes

### 4. Add Homepage Content
1. In theme editor, go to **Homepage**
2. Configure sections:
   - **Hero Banner**: Upload banner image (1920x1080px)
   - **Featured Collection**: Select your featured products collection
   - **Newsletter**: Enable if using email marketing

### 5. Configure Cart Settings
1. **Theme Settings** → **Cart**
2. Choose **Drawer** for slide-out cart (recommended)
3. Enable free shipping bar
4. Set threshold amount (e.g., $50)

### 6. Add Products
If you haven't already:
1. **Products** → **Add product**
2. Upload product images (2400x3600px recommended)
3. Add titles, descriptions, prices
4. Set inventory
5. Organize into collections

### 7. Set Up Footer
1. In theme editor: **Footer** section
2. Add footer menus
3. Add social media links:
   - **Theme Settings** → **Social Media**
   - Paste Instagram, Facebook, TikTok URLs

---

## Essential Optimizations

### Image Optimization
**Before uploading images:**
```bash
# Compress with online tools:
- TinyPNG (tinypng.com)
- Squoosh (squoosh.app)
- ImageOptim (imageoptim.com)

# Target sizes:
- Product images: 2400x3600px, <500KB
- Hero banners: 1920x1080px, <800KB
- Thumbnails: 600x900px, <200KB
```

### SEO Setup (Critical!)
1. **Settings** → **General**
2. Set store description (155 characters)
3. Add homepage title
4. **Online Store** → **Preferences**
5. Add Google Analytics tracking ID
6. Submit sitemap to Google Search Console:
   - Sitemap URL: `yourstore.com/sitemap.xml`

### Performance Check
1. Test on **Google PageSpeed Insights**
   - Target: 90+ on mobile
2. Test on **GTmetrix**
   - Target: Grade A
3. Test mobile responsiveness:
   - Chrome DevTools → Toggle device toolbar
   - Test on real iPhone/Android

---

## Troubleshooting

### Problem: Theme not appearing after upload
**Solution:**
- Check ZIP file contains all folders (assets, config, layout, etc.)
- Re-upload with correct folder structure
- Clear browser cache

### Problem: Images not showing
**Solution:**
- Re-upload images in theme editor
- Check file format (JPG, PNG, WebP only)
- Ensure images are <20MB

### Problem: Colors not changing
**Solution:**
- Go to Theme Settings → Colors
- Click **Save** after making changes
- Hard refresh browser (Ctrl+Shift+R / Cmd+Shift+R)

### Problem: Cart drawer not opening
**Solution:**
- Disable conflicting apps temporarily
- Check browser console for errors (F12)
- Ensure JavaScript is enabled

### Problem: Mobile menu not working
**Solution:**
- Clear site cache
- Disable browser extensions
- Test in incognito mode

---

## Next Steps

### Week 1: Content Population
- [ ] Upload all product images
- [ ] Write product descriptions
- [ ] Create collections (New Arrivals, Best Sellers, Sale)
- [ ] Add blog posts
- [ ] Set up pages (About, Contact, Shipping, Returns)

### Week 2: Marketing Setup
- [ ] Configure email marketing (Klaviyo/Mailchimp)
- [ ] Set up Facebook/Instagram shopping
- [ ] Install review app (Judge.me/Loox)
- [ ] Configure abandoned cart emails
- [ ] Set up discount codes

### Week 3: Legal & Policies
- [ ] Add Privacy Policy
- [ ] Add Terms of Service
- [ ] Add Refund Policy
- [ ] Add Shipping Policy
- [ ] Configure GDPR settings (if EU customers)

### Week 4: Launch Prep
- [ ] Test checkout process
- [ ] Test on multiple devices
- [ ] Set up payment gateways
- [ ] Configure shipping rates
- [ ] Create launch announcement
- [ ] Schedule social media posts

---

## Support Resources

### Documentation
- **Shopify Help Center**: help.shopify.com
- **Theme Documentation**: Included in README.md
- **Liquid Reference**: shopify.dev/api/liquid

### Community
- **Shopify Community**: community.shopify.com
- **Discord**: Various Shopify development servers
- **Reddit**: r/shopify

### Professional Help
If you need custom development:
- **Shopify Experts**: experts.shopify.com
- **Upwork/Fiverr**: Shopify theme developers
- **Storetasker**: On-demand Shopify experts

---

## Performance Benchmarks

After installation, your store should achieve:
- ✅ PageSpeed Mobile: 90-95
- ✅ PageSpeed Desktop: 95-100
- ✅ First Contentful Paint: <1.5s
- ✅ Time to Interactive: <2.5s
- ✅ Cumulative Layout Shift: <0.1

If not meeting these benchmarks:
1. Compress all images
2. Limit apps to essential only
3. Remove unused theme sections
4. Enable lazy loading
5. Use Shopify CDN (automatic)

---

## Security Checklist

Before going live:
- [ ] SSL certificate enabled (free with Shopify)
- [ ] Strong admin password
- [ ] Two-factor authentication enabled
- [ ] Staff accounts have appropriate permissions
- [ ] Customer data privacy settings configured
- [ ] Spam protection enabled on forms

---

## Backup & Version Control

**Before making major changes:**
1. **Online Store** → **Themes**
2. Click **Actions** → **Duplicate**
3. Name it: "Luxe Backup - [Date]"

**For developers using Git:**
```bash
git init
git add .
git commit -m "Initial theme setup"
git remote add origin your-repo-url
git push -u origin main
```

---

## 🎯 Launch Checklist

Final checks before launch:
- [ ] All products added with images
- [ ] Collections organized
- [ ] Navigation menus working
- [ ] Logo uploaded
- [ ] Colors match brand
- [ ] Footer links working
- [ ] Contact form tested
- [ ] Cart/checkout tested
- [ ] Mobile view checked
- [ ] SEO settings complete
- [ ] Analytics installed
- [ ] Social links added
- [ ] Legal pages added
- [ ] Payment gateway tested
- [ ] Shipping rates configured

---

## 🎉 You're Ready to Launch!

**Need help?** Reference the full README.md for detailed documentation.

**Found a bug?** Contact support with:
- Description of issue
- Browser/device used
- Screenshot
- Steps to reproduce

---

**Theme Version:** 1.0.0  
**Last Updated:** March 16, 2026  
**Shopify Compatibility:** Online Store 2.0
