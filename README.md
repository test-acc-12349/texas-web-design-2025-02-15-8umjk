# Texas Web Design Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Texas Web Design landing page. Whether you're new to web development or need a quick reference, you'll find step-by-step guidance for common maintenance tasks.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Original -->
<div class="text-2xl font-bold text-blue-600">TWD</div>

<!-- How to modify -->
<div class="text-2xl font-bold text-blue-600">Your Company Name</div>
```

#### Hero Section
The hero section contains the main headline and subheading:
```html
<h1 class="text-4xl md:text-6xl font-bold text-white mb-6">Texas Web Design</h1>
<p class="text-xl md:text-2xl text-white mb-8">Best Websites In Texas</p>
```
To update, simply replace the text between the tags while maintaining the HTML structure.

### Tailwind CSS Classes Explained

#### Responsive Design Classes
- `md:` prefix indicates styles that apply on medium screens and larger
- Example: `text-4xl md:text-6xl` means:
  - `text-4xl` on mobile (default)
  - `text-6xl` on medium screens and up

#### Common Class Patterns
```html
<!-- Spacing -->
mb-6    <!-- Margin bottom: 1.5rem -->
px-6    <!-- Padding left/right: 1.5rem -->
py-24   <!-- Padding top/bottom: 6rem -->

<!-- Colors -->
text-blue-600    <!-- Text color -->
bg-white         <!-- Background color -->

<!-- Typography -->
text-2xl         <!-- Font size -->
font-bold        <!-- Font weight -->
```

## Fixing Broken Links

### Navigation Menu Links
Current navigation links in the header:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#video">Watch</a>
    <a href="#faq">FAQ</a>
</div>
```

To update:
1. Locate the `href` attribute
2. Replace the value with your desired URL
3. For internal links, use `#section-id`
4. For external links, use full URLs starting with `https://`

### Call-to-Action Links
```html
<!-- Original -->
<a href="https://twd.com" class="inline-block bg-blue-600...">

<!-- Update to your domain -->
<a href="https://yourcompany.com" class="inline-block bg-blue-600...">
```

## Linking Privacy and Terms Pages

### Footer Legal Section
Locate the legal section in the footer:
```html
<div>
    <h3 class="text-xl font-bold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-blue-400">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-blue-400">Terms of Service</a></li>
        <li><a href="#" class="hover:text-blue-400">Cookie Policy</a></li>
    </ul>
</div>
```

To add proper links:
1. Create your privacy.html and terms.html pages
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-blue-400">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-blue-400">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Internal Links**
   - Ensure section IDs match href values
   - Check for typos in IDs
   - IDs are case-sensitive

2. **Responsive Design Issues**
   - Check mobile view using browser dev tools
   - Verify `md:` classes are properly applied
   - Test at different screen sizes

3. **Missing Icons**
   - Verify Font Awesome is properly loaded
   - Check icon class names against Font Awesome documentation
   - Ensure internet connectivity for CDN access

### Best Practices

1. Always backup your HTML before making changes
2. Test all links after updating
3. View changes in multiple browsers
4. Check mobile responsiveness
5. Validate HTML using W3C Validator

Need additional help? Contact our support team at admin@twd.com.

---

This guide is maintained by Texas Web Design. Last updated: 2024.