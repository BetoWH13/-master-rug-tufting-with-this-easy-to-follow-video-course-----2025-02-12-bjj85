# Rug Tufting Landing Page - Maintenance Guide

This guide will help you maintain and customize the Rug Tufting landing page. Whether you're new to web development or need a quick reference, follow these instructions to make common updates.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the site logo and navigation menu. To modify:

1. **Logo Text**: Find this section in the header:
```html
<div class="text-2xl font-bold bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">
    Tufting.xyz
</div>
```
Replace "Tufting.xyz" with your desired text.

2. **Navigation Menu Items**: Locate the navigation div:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```
Edit the text between `<a>` tags to change menu items.

### Hero Section
The main banner section can be updated here:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-8 leading-tight">
    🧶 Master Rug Tufting with This Easy-to-Follow Video Course!
</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12 max-w-3xl mx-auto">
    Learn Rug Tufting & Create Custom Rugs Like a Pro!
</p>
```

**Tailwind CSS Tips:**
- `text-4xl` to `text-6xl`: Controls text size at different screen sizes
- `md:` prefix: Applies styles on medium screens and larger
- `mb-8`: Adds margin bottom (spacing)
- `max-w-3xl`: Limits maximum width

### Features Section
To modify feature cards, locate this structure:
```html
<div class="bg-gray-900 p-8 rounded-xl hover:scale-105 transition duration-300">
    <i class="fas fa-video text-4xl text-purple-500 mb-4"></i>
    <h3 class="text-xl font-semibold mb-4">Step-by-step Video Lessons</h3>
    <p class="text-gray-400">Comprehensive video tutorials...</p>
</div>
```

## Managing Links

### Navigation Links
1. Internal links use hashtags (#) to scroll to sections:
```html
<a href="#features">Features</a>
```
To link to a new page instead, replace with:
```html
<a href="newpage.html">Features</a>
```

### Call-to-Action Buttons
Update the enrollment links:
```html
<a href="https://www.digistore24.com/redir/524735/BetoWH72/">
```
Replace the URL with your course enrollment link.

### Footer Links
Check and update all footer links:
```html
<ul class="space-y-2 text-gray-400">
    <li><a href="#features">Features</a></li>
    <li><a href="#benefits">Benefits</a></li>
    <li><a href="#faq">FAQ</a></li>
</ul>
```

## Adding Privacy and Terms Pages

1. Create new HTML files:
   - `privacy.html`
   - `terms.html`

2. Update footer links:
```html
<!-- Find this section in the footer -->
<ul class="space-y-2 text-gray-400">
    <li><a href="privacy.html" class="hover:text-purple-400 transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="terms.html" class="hover:text-purple-400 transition-colors duration-300">Terms of Service</a></li>
</ul>
```

3. Ensure consistent styling by copying these classes to new page links:
   - `hover:text-purple-400`
   - `transition-colors`
   - `duration-300`

## Troubleshooting

### Common Issues

1. **Broken Links**
   - Check for typos in `href` attributes
   - Ensure linked files exist in the correct directory
   - Test all links after updating

2. **Styling Problems**
   - Verify Tailwind CSS classes are spelled correctly
   - Check for missing closing tags
   - Maintain responsive prefixes (`md:`, `lg:`)

3. **Icon Issues**
   - Confirm Font Awesome is properly loaded
   - Check icon class names in the [Font Awesome documentation](https://fontawesome.com/icons)

### Need Help?
- Review the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Validate HTML at [W3C Validator](https://validator.w3.org/)
- Test responsiveness using browser developer tools

Remember to always backup your files before making changes, and test the page across different devices and browsers after updates.