# Image Download Guide

This guide will help you download and organize images from the original Grill Americano website.

## Quick Instructions

### Method 1: Manual Download (Recommended)

1. **Visit the original website**: https://grillamericano.com

2. **Download images**:
   - Right-click on any image
   - Select "Save Image As..." or "Download Image"
   - Save to appropriate folder in `/images/`

3. **Organize by type**:
   - **Logos** → `images/logos/`
   - **Hero/Banner images** → `images/hero/`
   - **Food photos** → `images/food/`
   - **Icons** → `images/icons/`

### Method 2: Browser DevTools

1. Open https://grillamericano.com
2. Right-click and select "Inspect" or press F12
3. Go to the "Network" tab
4. Filter by "Img" to see all images
5. Click on each image to view its URL
6. Download from the URL shown

### Method 3: Using wget (Command Line)

If you're comfortable with command line:

```bash
# Download a specific image
wget -P images/logos/ https://grillamericano.com/path/to/logo.svg

# Or use curl
curl -o images/hero/hero-bg.jpg https://grillamericano.com/path/to/image.jpg
```

## Key Images to Download

### Priority 1: Essential Images
- [ ] Main Grill Americano logo
- [ ] Melbourne location logo
- [ ] Sydney location logo
- [ ] Hero background image for homepage

### Priority 2: Content Images
- [ ] Food photography for homepage
- [ ] Location-specific images (Melbourne interior/exterior)
- [ ] Location-specific images (Sydney interior/exterior)

### Priority 3: Optional
- [ ] Additional food photography
- [ ] Menu item photos
- [ ] Event space photos
- [ ] Social media icons (if custom)

## Image Optimization

After downloading, optimize images for web:

### Using Online Tools
- **TinyPNG**: https://tinypng.com (for PNG/JPG)
- **Squoosh**: https://squoosh.app (Google's image optimizer)
- **SVGOMG**: https://jakearchibald.github.io/svgomg/ (for SVG files)

### Using Command Line Tools

**ImageMagick** (if installed):
```bash
# Resize and compress JPG
convert input.jpg -resize 1920x1080 -quality 85 output.jpg

# Convert to WebP
convert input.jpg -quality 80 output.webp
```

**cwebp** (for WebP conversion):
```bash
cwebp -q 80 input.jpg -o output.webp
```

## Updating HTML Files

After adding images, update the HTML files:

### Example: Hero Background

In `css/styles.css`, update line 34:
```css
.hero-section {
    background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
                url('../images/hero/hero-bg.jpg') center/cover no-repeat;
    background-color: #1a1a1a;
}
```

### Example: Logos

In `index.html` (and other pages), add logo images:
```html
<div class="flex items-center space-x-4 mb-8">
    <img src="images/logos/logo-melbourne.svg" alt="Melbourne" class="h-12">
    <img src="images/logos/logo-sydney.svg" alt="Sydney" class="h-12">
</div>
```

### Example: Food Photography

Add to sections in `index.html`:
```html
<div class="grid md:grid-cols-2 gap-8">
    <img src="images/food/steak.jpg" alt="Premium steak" class="w-full h-64 object-cover">
    <img src="images/food/interior.jpg" alt="Restaurant interior" class="w-full h-64 object-cover">
</div>
```

## Recommended Image Sizes

- **Hero backgrounds**: 1920x1080px (or larger)
- **Logos**: SVG preferred, or PNG at 300-500px width
- **Food photos**: 800x600px to 1200x900px
- **Icons**: 64x64px or SVG

## Legal Note

Ensure you have proper rights or permissions to use images from the original website. This replica is for educational/demonstration purposes. For production use, you would need:
- Original photography
- Licensed stock photos
- Permission from the website owner

## Alternative: Use Placeholder Images

If you can't download the original images, use placeholder services:

- **Unsplash**: https://unsplash.com (free food photography)
- **Pexels**: https://pexels.com (free stock photos)
- **Placeholder.com**: https://placeholder.com (for testing)

Example placeholder URLs:
```html
<!-- Temporary placeholder -->
<img src="https://via.placeholder.com/1200x600/262626/FFFFFF?text=Hero+Image" alt="Hero">
```

## Testing

After adding images:
1. Check all pages load correctly
2. Verify images are responsive (look good on mobile)
3. Test image loading speed
4. Ensure alt text is descriptive for accessibility
5. Check that images don't break layout

## Need Help?

If images don't appear:
1. Check file paths are correct (case-sensitive!)
2. Ensure images are in the right folders
3. Verify image file extensions match HTML (.jpg vs .jpeg)
4. Check browser console for 404 errors (F12 → Console)
