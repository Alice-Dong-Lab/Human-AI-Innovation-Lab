# Customization Guide for Human-AI Innovation Lab Website

## Quick Start Customization

Follow these steps to personalize the website for your lab:

### 1. Update Lab Information

**Files to edit:**
- `_config.yml` - Update title, description, author, and url
- `index.html` - Update hero section text and metadata
- All HTML files - Replace placeholder text with your content

### 2. Update Colors

**File:** `css/style.css`

Edit the CSS variables at the top:
```css
:root {
    --primary-color: #0066cc;      /* Main blue */
    --secondary-color: #1a1a1a;    /* Dark text/nav */
    --accent-color: #00a4e8;       /* Light blue */
    --light-bg: #f5f5f5;           /* Light background */
}
```

### 3. Add Team Members

**File:** `pages/team.html`

Add new team member cards:
```html
<div class="team-member">
    <div class="member-avatar">👨‍💻</div>
    <h3>John Doe</h3>
    <p class="title">Research Scientist</p>
    <p class="bio">Bio and research interests</p>
    <div class="member-links">
        <a href="https://twitter.com/"><i class="fab fa-twitter"></i></a>
        <a href="https://linkedin.com/"><i class="fab fa-linkedin"></i></a>
    </div>
</div>
```

### 4. Update Research Areas

**File:** `pages/research.html`

Edit the research project sections to match your lab's focus areas.

### 5. Add Publications

**File:** `pages/publications.html`

Add publication entries:
```html
<div class="publication">
    <h3>Paper Title</h3>
    <p class="authors"><strong>Authors:</strong> Your Name, Co-Author</p>
    <p class="venue"><strong>Venue:</strong> Journal/Conference Name, Year</p>
    <p class="abstract">Brief abstract...</p>
    <div class="pub-links">
        <a href="#" class="pub-link"><i class="fas fa-file-pdf"></i> PDF</a>
        <a href="#" class="pub-link"><i class="fas fa-code"></i> Code</a>
    </div>
</div>
```

### 6. Update Contact Information

**File:** `pages/contact.html`

Update:
- Address
- Email address
- Phone number
- GitHub link

### 7. Add Lab Logo

1. Create an `assets` folder in the root
2. Add your logo as `logo.png`
3. Update `index.html` navigation to include:
```html
<img src="assets/logo.png" alt="Lab Logo" style="height: 40px;">
```

### 8. Update Social Media Links

In all HTML files, update the footer social links:
```html
<a href="https://twitter.com/yourhandle" class="social-icon">
    <i class="fab fa-twitter"></i>
</a>
```

## Color Customization Examples

### Dark Theme
```css
--primary-color: #1e3a8a;      /* Dark blue */
--accent-color: #3b82f6;       /* Lighter blue */
--secondary-color: #0f172a;    /* Very dark */
```

### Green Theme
```css
--primary-color: #059669;      /* Teal */
--accent-color: #10b981;       /* Light green */
--secondary-color: #065f46;    /* Dark green */
```

### Purple Theme
```css
--primary-color: #7c3aed;      /* Purple */
--accent-color: #a78bfa;       /* Light purple */
--secondary-color: #4c1d95;    /* Dark purple */
```

## Adding More Pages

1. Create a new HTML file in `pages/` folder
2. Copy the structure from an existing page
3. Update the navigation menu in all files to link to new page
4. Style consistently with the existing design

## Local Testing

Before deploying, test locally:

```bash
# Python 3
python -m http.server 8000

# Then visit: http://localhost:8000
```

## Deployment

Once customized:
1. Commit all changes
2. Push to main branch
3. GitHub Pages will automatically deploy
4. Visit: `https://Alice-Dong-Lab.github.io/Human-AI-Innovation-Lab/`

## Need Help?

Refer to:
- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [HTML/CSS Resources](https://developer.mozilla.org/)
- [Font Awesome Icons](https://fontawesome.com/icons)
