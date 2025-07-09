# Landing Page Maintenance Guide

This guide will help you maintain and customize the Downers Grove Bathroom Remodeling landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Located at the top of the page -->
<a href="#" class="text-2xl font-bold">
    DG Remodeling  <!-- Change company name here -->
</a>
```

#### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-6 leading-tight">
    Luxury Bathroom Remodeling in Downers Grove, IL  <!-- Update main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12">
    Transform your bathroom...  <!-- Update subheadline -->
</p>
```

#### Contact Information
```html
<a href="tel:8775596432">Call (877) 559-6432 Today</a>  <!-- Update phone number -->
<a href="mailto:info@downersgrovebathremodel.com">  <!-- Update email address -->
```

### Tailwind CSS Classes Explained

#### Responsive Design Classes
- `md:` - Applies styles on medium screens (768px and up)
- `lg:` - Applies styles on large screens (1024px and up)
- Example:
  ```html
  <h1 class="text-4xl md:text-5xl lg:text-6xl">
  <!-- text-4xl (mobile) → text-5xl (tablet) → text-6xl (desktop) -->
  ```

#### Common Styling Classes
- Background colors: `bg-gray-900`, `bg-blue-600`
- Text colors: `text-white`, `text-gray-300`
- Padding: `p-8`, `py-24`, `px-4`
- Margin: `mb-6`, `mt-12`
- Hover effects: `hover:bg-blue-700`, `hover:scale-105`

### Modifying Styles
To change a section's background color:
```html
<!-- Original -->
<section class="bg-gray-800">

<!-- Modified (example) -->
<section class="bg-blue-800">
```

## 2. Fixing Broken Links

### Navigation Menu Links
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```
To update:
1. Identify the section ID you want to link to
2. Add `#` followed by the section ID in the `href` attribute
3. Example: `<a href="#new-section">New Section</a>`

### External Links
```html
<!-- Phone number -->
<a href="tel:8775596432">
<!-- Email -->
<a href="mailto:info@downersgrovebathremodel.com">
```
To update:
1. Replace phone number in both the `href` and displayed text
2. Update email address in both the `href` and displayed text

## 3. Linking Privacy and Terms Pages

### Footer Links Section
```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Create privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
```

## Troubleshooting Tips

### Common Issues and Solutions

1. **Broken Internal Links**
   - Ensure section IDs match exactly with href attributes
   - Check for typos in IDs
   - IDs must be unique across the page

2. **Responsive Design Issues**
   - Test at different screen sizes using browser dev tools
   - Verify `md:` and `lg:` classes are properly set
   - Check container widths with `container mx-auto`

3. **Style Inconsistencies**
   - Maintain color scheme using existing Tailwind classes
   - Keep consistent spacing using similar padding/margin values
   - Follow existing hover effect patterns

### Quick Fixes

```html
<!-- Fix misaligned content -->
<div class="container mx-auto px-4">

<!-- Fix spacing issues -->
<section class="py-24">  <!-- Consistent vertical padding -->

<!-- Fix hover effects -->
<a class="hover:text-blue-400 transition duration-300">
```

## Best Practices

1. Always maintain the responsive design structure
2. Keep consistent spacing throughout sections
3. Test all links after making changes
4. Preserve the existing color scheme
5. Back up files before making major changes

Remember to test all changes across different devices and browsers to ensure consistency in appearance and functionality.