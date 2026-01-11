# Personal Resume Website

A professional, responsive personal website designed to serve as an online resume and portfolio. This website showcases your skills, experience, education, projects, and provides a way for potential employers or clients to contact you.

## ✨ Features

### 📄 Complete Resume Sections
- **Hero Section**: Eye-catching introduction with your name, tagline, and call-to-action buttons
- **About Me**: Detailed overview of your background, interests, and professional statistics
- **Work Experience**: Timeline-based display of your career history with detailed descriptions
- **Education**: Academic qualifications and professional certifications
- **Skills & Technologies**: Organized showcase of your technical skills across different categories
- **Featured Projects**: Portfolio section highlighting your best work with images and descriptions
- **Contact Section**: Multiple ways to get in touch, including a functional contact form

### 🎨 Design Features
- Modern gradient color scheme (purple/blue)
- Clean, professional layout
- Smooth animations and transitions
- Interactive hover effects
- Font Awesome icons throughout

### 📱 Responsive Design
- Mobile-first approach
- Fully responsive on all devices (phones, tablets, desktops)
- Hamburger menu for mobile navigation
- Optimized layouts for different screen sizes

### ♿ Accessibility Features
- Semantic HTML5 markup
- ARIA labels and roles for screen readers
- Proper heading hierarchy
- Descriptive alt text for all images
- Keyboard navigation support
- Form labels for all inputs
- Skip to main content functionality

### ⚡ Performance
- Lazy loading for images
- Optimized CSS and JavaScript
- Smooth scroll behavior
- Minimal external dependencies

## 🛠️ Technical Stack

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with Flexbox and Grid
- **JavaScript**: Interactive features and animations
- **Font Awesome**: Icon library

## 📂 File Structure

```
Personal Website/
│
├── index.html          # Main HTML file
├── style.css           # All CSS styles
├── script.js           # JavaScript functionality
└── README.md          # This file
```

## 🚀 Getting Started

### View the Website

1. **Local Viewing**: Simply open `index.html` in your web browser
2. **Live Server** (Recommended for development):
   - If using VS Code, install the "Live Server" extension
   - Right-click on `index.html` and select "Open with Live Server"

### Customize Your Website

#### 1. Personal Information
Update the following in `index.html`:

- **Name**: Replace "Your Name" with your actual name (appears in multiple places)
- **Tagline**: Update "Web Developer | Designer | Problem Solver" to match your role
- **Hero Description**: Modify the introduction text in the hero section

#### 2. About Section
- Update the about text paragraphs with your story
- Modify statistics (years of experience, projects completed, happy clients)

#### 3. Work Experience
For each job in the timeline:
- Update dates (use proper datetime format)
- Change job title and company name
- Modify description and achievements
- Add or remove jobs as needed

#### 4. Education
- Update degree information
- Change university name and graduation dates
- Add your actual certifications

#### 5. Skills
- Add or remove skills based on your expertise
- Organize into relevant categories
- Customize category names if needed

#### 6. Projects
For each project:
- Replace placeholder images with actual screenshots
- Update project titles and descriptions
- Change technology tags
- Add links to live demos and GitHub repositories
- Add or remove projects as needed

**To replace project images:**
```html
<img src="path/to/your/image.jpg" alt="Detailed description of project">
```

#### 7. Contact Information
Update in `index.html`:
- Email address
- Phone number
- Location (city, country)
- Social media links:
  - GitHub: `https://github.com/yourusername`
  - LinkedIn: `https://linkedin.com/in/yourusername`

#### 8. Colors and Styling
Modify CSS variables in `style.css`:

```css
:root {
    --primary-color: #667eea;      /* Main brand color */
    --secondary-color: #764ba2;    /* Secondary brand color */
    --text-color: #333;            /* Main text color */
    --text-light: #666;            /* Lighter text */
    --bg-color: #f8f9fa;          /* Background color */
}
```

## 📋 Technical Requirements Met

### ✅ HTML Standards
- Valid HTML5 markup
- Proper semantic elements (`header`, `main`, `section`, `article`, `nav`, `footer`)
- Appropriate use of heading hierarchy (h1-h4)
- Semantic time elements for dates
- Proper form structure with labels

### ✅ CSS Best Practices
- Valid CSS3
- Organized structure with clear sections
- CSS custom properties (variables) for theming
- BEM-like naming conventions
- Mobile-first responsive design
- CSS Grid and Flexbox for layouts

### ✅ Accessibility
- All images have descriptive alt text
- ARIA labels and roles where appropriate
- Proper form labels (visually hidden but accessible)
- Semantic HTML for better screen reader support
- Sufficient color contrast
- Keyboard navigation support

### ✅ Responsive Design
- Breakpoints for mobile, tablet, and desktop
- Flexible grid layouts
- Responsive images
- Mobile navigation menu
- Touch-friendly interactive elements

## 🎯 Features Implementation

### Smooth Scrolling
The website includes smooth scrolling navigation. Clicking any navigation link smoothly scrolls to the corresponding section.

### Mobile Menu
On mobile devices, the navigation collapses into a hamburger menu that slides in from the top when activated.

### Scroll Animations
Elements fade in and slide up as you scroll down the page, creating an engaging user experience.

### Counter Animation
Statistics in the About section animate from 0 to their final values when they come into view.

### Contact Form
The contact form includes:
- Client-side validation
- Placeholder demo functionality
- Proper labels for accessibility
- Required field indicators

**Note**: The form currently shows a demo alert. To make it functional, you'll need to:
1. Set up a backend service (Node.js, PHP, etc.)
2. Or use a form service like Formspree, Netlify Forms, or EmailJS
3. Update the form submission handler in `script.js`

## 🌐 Deployment Options

### Option 1: GitHub Pages (Free)
1. Create a GitHub repository
2. Push your files to the repository
3. Go to Settings > Pages
4. Select main branch as source
5. Your site will be live at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Free)
1. Create a Netlify account
2. Drag and drop your folder to Netlify
3. Your site will be live instantly with a custom URL

### Option 3: Vercel (Free)
1. Create a Vercel account
2. Import your GitHub repository or upload files
3. Deploy with one click

### Option 4: Traditional Web Hosting
Upload all files to your web host via FTP using FileZilla or similar tools.

## 🔧 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 Customization Tips

### Adding New Sections
1. Add the section in `index.html` following the existing structure
2. Add corresponding styles in `style.css`
3. Add navigation link in the navbar
4. Ensure proper semantic HTML and ARIA labels

### Changing Fonts
Add a Google Font to the `<head>` section:
```html
<link href="https://fonts.googleapis.com/css2?family=Your+Font&display=swap" rel="stylesheet">
```

Then update in `style.css`:
```css
body {
    font-family: 'Your Font', sans-serif;
}
```

### Adding More Projects
Copy an existing project card and modify:
```html
<article class="project-card">
    <!-- Project content -->
</article>
```

## 🐛 Troubleshooting

### Images Not Loading
- Check file paths are correct
- Ensure images are in the same directory or use correct relative paths
- Verify image file extensions match exactly

### Styles Not Applying
- Ensure `style.css` is in the same directory as `index.html`
- Check browser console for errors
- Clear browser cache

### JavaScript Not Working
- Ensure `script.js` is in the same directory as `index.html`
- Check browser console for errors
- Verify Font Awesome CDN is loading

## 📬 Contact Form Integration

To make the contact form functional, here are some options:

### Formspree (Easiest)
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### EmailJS
1. Sign up at emailjs.com
2. Follow their integration guide
3. Update the form handler in `script.js`

### Custom Backend
Create a server endpoint and update the form action or add AJAX submission.

## 📄 License

This is a personal project template. Feel free to use and modify it for your own personal website.

## 🤝 Contributing

This is a personal website template. Feel free to fork and customize for your own use!

## 💡 Tips for Success

1. **Keep it updated**: Regularly update your experience, skills, and projects
2. **Use real images**: Replace placeholder images with actual project screenshots
3. **Be authentic**: Write in your own voice in the about section
4. **Proofread**: Check for spelling and grammar errors
5. **Test thoroughly**: View your site on different devices and browsers
6. **SEO**: Update meta tags with your actual information
7. **Performance**: Optimize images before uploading (compress to reduce file size)

## 📞 Support

If you encounter any issues or have questions about customizing the website:
- Check browser console for errors
- Validate HTML at validator.w3.org
- Validate CSS at jigsaw.w3.org/css-validator
- Test accessibility with browser DevTools

---

**Good luck with your personal website! 🚀**
