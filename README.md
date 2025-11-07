# Dr. Paa Kwasi Adusei - Personal Website

A modern, minimalistic personal website showcasing Dr. Paa Kwasi Adusei's professional profile, research, and publications.

## Features

- **Minimalistic Light Theme Design** - Clean, professional aesthetic with a focus on readability
- **Fully Responsive** - Works seamlessly on desktop, tablet, and mobile devices
- **Smooth Animations** - Subtle fade-in effects and smooth scrolling
- **Interactive Navigation** - Fixed navigation bar with active section highlighting
- **Mobile-Friendly Menu** - Hamburger menu for mobile devices
- **Sections Include:**
  - Hero/Introduction
  - About & Education
  - Research & Expertise
  - Publications
  - Professional Experience
  - Contact Information

## Getting Started

### Viewing the Website

1. Simply open `index.html` in any modern web browser
2. No build process or dependencies required

### Customizing Content

#### Update Contact Information

Edit the following sections in `index.html`:

**Email** (line ~294):
```html
<p><a href="mailto:your.email@example.com">your.email@example.com</a></p>
```

**LinkedIn** (line ~308):
```html
<p><a href="#" target="_blank">linkedin.com/in/yourprofile</a></p>
```

#### Adding Publications

Replace the placeholder publication section (starting around line ~175) with actual publications:

```html
<div class="publication-item">
    <h3 class="publication-title">Your Publication Title</h3>
    <p class="publication-authors">Author 1, Author 2, P.K. Adusei, Author 3</p>
    <p class="publication-venue">Journal Name, Volume(Issue), Pages, Year</p>
    <p class="publication-abstract">Brief abstract or description of the publication...</p>
    <div class="publication-links">
        <a href="path/to/paper.pdf" class="publication-link">PDF</a>
        <a href="https://doi.org/..." class="publication-link">DOI</a>
    </div>
</div>
```

#### Adding Professional Experience

Update the experience timeline section (starting around line ~209) with specific positions:

```html
<div class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
        <h3>Position Title</h3>
        <p class="timeline-company">Company Name</p>
        <p class="timeline-period">Start Date - End Date</p>
        <ul class="timeline-description">
            <li>Key achievement or responsibility 1</li>
            <li>Key achievement or responsibility 2</li>
            <li>Key achievement or responsibility 3</li>
        </ul>
    </div>
</div>
```

#### Adding a Profile Photo

Add a profile photo to the hero section:

1. Place your photo in the project directory (e.g., `profile.jpg`)
2. Add the image to the hero section in `index.html`:

```html
<div class="hero-content">
    <img src="profile.jpg" alt="Dr. Paa Kwasi Adusei" class="profile-photo">
    <h1 class="hero-title">Dr. Paa Kwasi Adusei</h1>
    <!-- rest of content -->
</div>
```

3. Add styling to `styles.css`:

```css
.profile-photo {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    object-fit: cover;
    margin: 0 auto var(--spacing-lg);
    border: 4px solid var(--border-color);
    box-shadow: var(--shadow-lg);
}
```

### Color Customization

To change the color scheme, edit the CSS variables in `styles.css` (lines 11-23):

```css
:root {
    --primary-color: #2563eb;  /* Main blue color */
    --primary-dark: #1e40af;   /* Darker shade */
    --primary-light: #3b82f6;  /* Lighter shade */
    /* ... */
}
```

## File Structure

```
paa_kwesi_adusei/
├── index.html          # Main HTML file
├── styles.css          # All styling and responsive design
├── script.js           # Interactive features and animations
└── README.md           # This file
```

## Browser Compatibility

Works on all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Deployment

### GitHub Pages

1. Create a GitHub repository
2. Upload all files (index.html, styles.css, script.js)
3. Go to Settings > Pages
4. Select main branch as source
5. Your site will be available at `https://username.github.io/repository-name`

### Netlify

1. Drag and drop the project folder to [Netlify Drop](https://app.netlify.com/drop)
2. Your site will be live instantly with a custom URL

### Custom Domain

Both GitHub Pages and Netlify support custom domains. Simply:
1. Purchase a domain
2. Follow the platform's instructions to connect your domain
3. Update DNS settings as directed

## Adding New Features

### Contact Form

To add a working contact form, consider using:
- [Formspree](https://formspree.io/)
- [Netlify Forms](https://www.netlify.com/products/forms/)
- [Google Forms](https://www.google.com/forms/)

### Analytics

Add Google Analytics by inserting this in the `<head>` section of `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR-GA-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR-GA-ID');
</script>
```

### Blog Section

To add a blog, consider integrating:
- [Jekyll](https://jekyllrb.com/) for static blog
- [Medium](https://medium.com/) embed
- Custom blog page with similar styling

## License

This website template is free to use and modify for personal purposes.

## Support

For questions or issues with the website, please contact the developer or create an issue in the repository.

---

**Last Updated:** January 2025
