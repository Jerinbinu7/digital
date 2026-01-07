# Zentra Marketing Agency - Setup Guide

## 📞 How to Update Phone Numbers

### Current Placeholder Numbers
The website currently uses placeholder numbers: `919876543210`

### Where to Update:
You need to replace `919876543210` with your actual WhatsApp number in these files:
- `index.html` (3 places)
- `about.html` (2 places)
- `work.html` (2 places)
- `services.html` (2 places)
- `contact.html` (4 places)

### Format:
- **WhatsApp Link**: `https://wa.me/91XXXXXXXXXX` (no +, no spaces, just country code + number)
- **Phone Link**: `tel:+91-XXXXXXXXXX` (with + and dashes for formatting)

### Example:
If your number is: **9876543210**
- WhatsApp: `https://wa.me/919876543210`
- Phone: `tel:+91-98765-43210`

---

## 🖼️ How to Add Images

### Step 1: Create Images Folder
Create a folder called `images` in your project root:
```
bank/
  ├── images/
  │   ├── hero/
  │   ├── work/
  │   ├── team/
  │   └── logo/
  ├── index.html
  └── ...
```

### Step 2: Add Your Images
Place your images in the appropriate folders:
- **Hero images**: `images/hero/`
- **Work/Case study images**: `images/work/`
- **Team photos**: `images/team/`
- **Logo**: `images/logo/`

### Step 3: Update HTML with Images

#### A. Hero Section Image (Optional)
In `index.html`, you can add a hero image:
```html
<section class="hero">
    <div class="container">
        <div class="hero-content">
            <!-- Add image before or after hero-content -->
            <img src="images/hero/hero-image.jpg" alt="Zentra Marketing Agency" class="hero-image">
            <!-- Rest of hero content -->
        </div>
    </div>
</section>
```

#### B. Work/Case Study Images
In `work.html`, replace the placeholder divs with actual images:

**Current (placeholder):**
```html
<div class="work-image-placeholder">
    <span>Grid Facade Interior</span>
</div>
```

**Replace with:**
```html
<img src="images/work/grid-facade.jpg" alt="Grid Facade Interior Project" class="work-image">
```

**Update CSS** - Add this to `styles.css`:
```css
.work-image {
    width: 100%;
    height: 300px;
    object-fit: cover;
    border-radius: 4px 4px 0 0;
}
```

#### C. Service Icons (Optional)
Replace emoji icons with image icons:
```html
<!-- Instead of: -->
<div class="service-icon">📱</div>

<!-- Use: -->
<img src="images/icons/social-media.svg" alt="Social Media" class="service-icon">
```

#### D. Logo
Add a logo image to navigation:
```html
<a href="index.html" class="logo">
    <img src="images/logo/zentra-logo.svg" alt="Zentra" class="logo-image">
</a>
```

### Image Optimization Tips:
1. **Format**: Use WebP or JPG for photos, SVG for icons
2. **Size**: Keep images under 500KB
3. **Dimensions**: 
   - Hero images: 1920x1080px
   - Work images: 1200x800px
   - Team photos: 600x600px
4. **Tools**: Use TinyPNG or Squoosh to compress images

---

## 🌐 How to Make the Website Live

### Option 1: Netlify (Recommended - Free & Easy)

1. **Create Netlify Account**
   - Go to [netlify.com](https://netlify.com)
   - Sign up with GitHub/Email

2. **Deploy**
   - Drag and drop your entire `bank` folder to Netlify dashboard
   - OR connect to GitHub and push your code

3. **Custom Domain** (Optional)
   - Add your domain in Netlify settings
   - Update DNS records as instructed

**Pros**: Free, automatic HTTPS, fast CDN, easy updates

---

### Option 2: Vercel (Free & Fast)

1. **Create Vercel Account**
   - Go to [vercel.com](https://vercel.com)
   - Sign up with GitHub

2. **Deploy**
   - Install Vercel CLI: `npm i -g vercel`
   - Run `vercel` in your project folder
   - Follow prompts

**Pros**: Free, excellent performance, easy GitHub integration

---

### Option 3: GitHub Pages (Free)

1. **Create GitHub Repository**
   - Create new repo on GitHub
   - Upload all files

2. **Enable GitHub Pages**
   - Go to Settings > Pages
   - Select main branch
   - Your site will be at: `username.github.io/repo-name`

**Pros**: Free, version control built-in

---

### Option 4: Traditional Web Hosting

1. **Buy Hosting**
   - Popular options: Hostinger, Bluehost, SiteGround
   - Get a domain name (e.g., zentramarketing.com)

2. **Upload Files**
   - Use FTP (FileZilla) or cPanel File Manager
   - Upload all HTML, CSS, JS files
   - Upload images folder

3. **Configure**
   - Point domain to hosting
   - Set up SSL certificate (HTTPS)

---

## 📧 Update Email Address

In `contact.html`, find and replace:
```html
<a href="mailto:hello@zentramarketing.com" class="btn btn-outline">Send Email</a>
```

Replace `hello@zentramarketing.com` with your actual email.

---

## ✅ Pre-Launch Checklist

- [ ] Update all phone numbers
- [ ] Update email address
- [ ] Add real images (remove placeholders)
- [ ] Test all links (WhatsApp, phone, email)
- [ ] Test contact form (connect to backend)
- [ ] Test on mobile devices
- [ ] Check all pages load correctly
- [ ] Verify SEO meta tags
- [ ] Add Google Analytics (optional)
- [ ] Set up domain and hosting
- [ ] Test website speed
- [ ] Check for broken links

---

## 🔧 Contact Form Setup

The contact form currently just shows a success message. To make it work:

### Option 1: Formspree (Easiest)
1. Sign up at [formspree.io](https://formspree.io)
2. Get your form endpoint
3. Update `contact.html` form action:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 2: EmailJS (Free)
1. Sign up at [emailjs.com](https://emailjs.com)
2. Follow their setup guide
3. Update `script.js` with EmailJS code

### Option 3: Backend API
Connect to your own backend/API endpoint.

---

## 📱 Quick Phone Number Update Script

If you want to update all phone numbers at once, use Find & Replace in your code editor:

**Find**: `919876543210`
**Replace**: `YOUR_ACTUAL_NUMBER` (e.g., `919876543210`)

**Find**: `+91 98765 43210`
**Replace**: `+91-XXXXX-XXXXX` (formatted version)

---

## 🚀 Recommended Hosting for Kerala Businesses

1. **Hostinger** - Good for Indian businesses, affordable
2. **Netlify** - Best for static sites, free tier
3. **Vercel** - Fast, free, great performance

---

## Need Help?

- Check all HTML files for phone numbers
- Test locally first (open index.html in browser)
- Use browser DevTools to check for errors
- Validate HTML at [validator.w3.org](https://validator.w3.org)


