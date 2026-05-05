# Contact Form Integration Guide

## Overview

I've integrated a contact form into your Medieval Seals conference website that maintains the "Tactile Minimalism" aesthetic of your design system. The form uses **Formspree**, a free service that handles form submissions without requiring any backend code.

---

## What Changed

### 1. **HTML Contact Section** (index.html)

The contact section now includes:
- A fully functional contact form with fields for Name, Email, Subject, and Message
- Form validation (all fields are required)
- Placeholder text to guide users
- A decorative separator dividing the form from contact info
- Direct contact information for Dr. John McEwan

### 2. **CSS Form Styling** (styles.css)

All form styling follows your design system:

#### **Form Fields**
- Minimalist **underline-only inputs** that evoke "ruled lines on a page" (per DESIGN.md)
- Labels styled in **uppercase, small caps** matching your `.label-sm` typography
- Inputs transition to **Antique Gold (#7b5811)** on focus
- Transparent backgrounds maintain the parchment aesthetic
- Proper spacing using your 8px baseline grid

#### **Visual Hierarchy**
- Labels: Deep Ink Blue (#001022), 13px uppercase
- Input text: On-surface color (#1c1c15)
- Placeholders: Subtle gray (outline color)
- Border color transitions: Outline-variant → Secondary gold on focus

#### **Responsive Design**
- Mobile-optimized with 16px input font size (prevents iOS zoom)
- Adjusted spacing for smaller screens
- Contact info stacks vertically on mobile

#### **Submit Button**
- Uses your existing `.btn-seal` wax-seal gradient styling
- Full-width on desktop, centered content
- Maintains hover scale animation

---

## How to Set Up Formspree

Formspree is a free service that processes form submissions. Here's how to configure it:

### **Step 1: Create a Formspree Account**
1. Go to **[formspree.io](https://formspree.io)**
2. Sign up with your email
3. Create a new form for your project

### **Step 2: Get Your Form ID**
1. After creating the form, you'll receive a unique Form ID (e.g., `f_abc123xyz`)
2. Copy this ID

### **Step 3: Update the Form Action**
In `index.html`, find this line in the contact form:

```html
<form action="https://formspree.io/f/xyzabc123" method="POST" class="contact-form">
```

Replace `xyzabc123` with your actual Formspree Form ID. Example:

```html
<form action="https://formspree.io/f/abc123xyz" method="POST" class="contact-form">
```

### **Step 4: Test the Form**
1. Fill out the form on your website
2. Submit it
3. Formspree will send you a confirmation email the first time
4. Click the link to activate the form
5. Future submissions will be sent directly to your email

### **Step 5: (Optional) Configure Formspree Settings**
In your Formspree dashboard, you can:
- Set a custom "thank you" redirect page
- Add automatic email responses
- Set up email notifications
- Customize the form appearance

---

## Design System Integration

### **Typographic Hierarchy**

```
Labels (13px, uppercase, Deep Ink Blue)
    ↓
Input Text (16px, Newsreader, On-surface)
    ↓
Placeholders (14px, subtle gray)
```

### **Color Transitions**

| State | Color | Purpose |
|-------|-------|---------|
| Default border | Outline-variant (#c4c6cd) | Subtle, minimal |
| Focused border | Secondary (#7b5811) | Gold accent on interaction |
| Label text | Primary (#001022) | Deep ink blue, authoritative |
| Placeholder | Outline (#74777d) | Subtle guidance |

### **Spacing (8px Grid)**

- Form group margin-bottom: 28px (3.5 units)
- Label margin-bottom: 12px (1.5 units)
- Input padding: 12px vertical (1.5 units)
- Submit button margin-top: 32px (4 units)

### **Rounded Corners**

Form fields use `border-radius: none` (underline only) to maintain the minimal, "ruled page" aesthetic. The submit button uses `.btn-seal` class which applies `border-radius: var(--radius-full)` (9999px) for the wax seal appearance.

---

## CSS Classes Added

### **New Classes**
- `.contact-header` — Container for form title and intro text
- `.contact-intro` — Introduction paragraph styling
- `.contact-form` — Form wrapper
- `.form-group` — Individual form field container
- `.contact-divider` — Decorative separator between form and contact info
- `.contact-info` — Direct contact information section
- `.contact-info-label` — Label for contact info section

### **Existing Classes Retained**
- `.contact` — Section background and padding
- `.contact-card` — Card container
- `.contact-detail` — Contact person layout
- `.contact-detail-icon` — Icon styling
- `.contact-detail-value` — Contact name styling
- `.btn-seal` — Wax seal button (used for submit)

---

## Features

✅ **Fully Functional** — Form submissions are sent directly to your email via Formspree  
✅ **No Backend Required** — Pure HTML + CSS, no server code needed  
✅ **Email Obfuscation** — Email address is never exposed on the page (only in form results)  
✅ **Accessible** — Proper label associations, keyboard navigation support  
✅ **Responsive** — Mobile-optimized with proper font sizes to prevent iOS zoom  
✅ **On-Brand** — Consistent with your Medieval Scholarly System aesthetic  
✅ **Performant** — Minimal CSS, no heavy JavaScript or external libraries  

---

## Form Fields

The contact form includes four fields:

1. **Full Name** (text input, required)
2. **Email Address** (email input, required, HTML5 validation)
3. **Subject** (text input, required)
4. **Message** (textarea, 6 rows, required)

All fields have:
- Placeholder text for guidance
- Required validation (HTML5)
- Proper label associations for accessibility
- Consistent styling

---

## Optional Enhancements

### **Add Custom Success Message**
Configure in Formspree dashboard → Redirects → set custom "Thank you" page URL

### **Add Auto-Reply Email**
In Formspree, set up an automatic response email sent to form submitters

### **Add Subject Line to Emails**
The form already captures a "Subject" field which will appear in your email notifications

### **Spam Protection**
Formspree includes built-in spam filtering. You can also enable CAPTCHA in dashboard settings.

---

## Troubleshooting

### **Form not submitting?**
1. Check that the Form ID in the action URL is correct
2. Make sure you activated the form via the confirmation email from Formspree
3. Check browser console for any JavaScript errors

### **Emails not arriving?**
1. Check your spam/junk folder
2. Verify the email address in Formspree settings matches your actual email
3. In Formspree dashboard, check the "Submissions" tab to see if the form was received

### **Styling looks off?**
1. Make sure the updated `styles.css` is linked in your HTML
2. Clear browser cache (Ctrl+Shift+Delete or Cmd+Shift+Delete)
3. Check that no CSS file changes were overwritten

---

## Browser Compatibility

The form works in all modern browsers:
- Chrome/Edge 88+
- Firefox 87+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## Files Provided

- **index.html** — Updated with contact form
- **styles.css** — Updated with complete form styling
- **FORM_INTEGRATION_GUIDE.md** — This file

---

## Next Steps

1. ✅ Copy the updated `index.html` and `styles.css` to your project
2. ✅ Create a Formspree account and get your Form ID
3. ✅ Update the form `action` URL with your Form ID
4. ✅ Test the form by submitting a test message
5. ✅ Activate the form via confirmation email
6. ✅ Deploy to your server

---

## Support

**Formspree Documentation:** https://formspree.io/docs/  
**Design System Reference:** See DESIGN.md for typography, colors, and component guidelines
