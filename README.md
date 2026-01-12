# Annamarie Nieuwoudt - Personal Portfolio Website

A minimalist retro-futuristic personal portfolio website showcasing professional experience, skills, projects, and creative work. Built with a cyberpunk-inspired design system featuring neon colors, geometric shapes, and animated effects.

## 🎨 Design System

### Visual Style
This website features a **minimalist retro-futuristic aesthetic** inspired by cyberpunk and sci-fi interfaces:

- **Color Palette**: Neon cyan (#00ffff), magenta (#ff00ff), and neon green (#00ff88) against dark backgrounds (#0a0a0f)
- **Typography**: Orbitron (geometric headers) and Rajdhani (clean body text) from Google Fonts
- **Visual Effects**: 
  - Scanline overlay animation for CRT monitor effect
  - Grid background patterns
  - Polygon clip-path shapes on cards and buttons
  - Neon glow effects on hover
  - Glitch animations on active elements
- **Components**: Geometric cards, timeline visualizations, hover-reactive project cards, neon-bordered sections

### Design Features
- Consistent neon glow effects across interactive elements
- Animated scanlines creating a retro-tech atmosphere
- Clipped polygon borders (15px cuts on corners) for geometric aesthetic
- Pulsing dot animations on timeline items
- Smooth hover transforms with scale and glow effects

## 🛠️ Technical Stack

- **HTML5**: Semantic markup with accessibility features
- **CSS3**: Custom design system with animations, Grid, and Flexbox
- **JavaScript**: Smooth scrolling, mobile menu, scroll animations
- **Font Awesome 6.4.0**: Icon library
- **Google Fonts**: Orbitron (400/500/700/900), Rajdhani (300/400/500/600/700)

## 📂 Project Structure

```
Personal Website/
│
├── index.html                      # Main portfolio page
├── style.css                       # Complete design system (~1024 lines)
├── script.js                       # Interactive functionality
├── README.md                       # This file
│
├── photography.html                # Photography portfolio gallery
├── logo-design.html                # Logo design gallery
├── marketing-materials.html        # Graphic design & marketing gallery (merged with social media)
├── mockups.html                    # Product mockup showcase
├── sustainable-projects.html       # Detailed volunteering project page with photo gallery
├── social-media.html              # (Legacy - content merged into marketing-materials.html)
│
└── Images/                         # All image assets
    ├── photography/                # Nature & wildlife photos
    ├── logos/                      # Logo design work
    ├── marketing/                  # Flyers, business cards, social media posts
    ├── mockups/                    # Product mockup renders
    ├── Dalmada Water.png          # NGO project showcase image
    └── [various project images]
```

## 🌟 Key Sections

### Hero Section
- Animated name with neon glow effect
- Highlighted text with glowing cyan accent
- Two CTA buttons: Portfolio and Contact (with geometric styling)

### About Section
- Professional summary aligned with CV
- Statistics cards with icons (experience, projects, skills)
- Retro-futuristic card design with clipped corners

### Resume Section
Comprehensive professional background divided into:

1. **Education**
   - BS Computer Information Systems (Grand Canyon University, 2025)
   - AS Graphic Communications (Aims Community College, 2018)
   - Azure Cloud Fundamentals (in progress)
   - AI Prompt Engineering coursework

2. **Experience**
   - Timeline layout with glowing dots
   - Multiple positions from 2012-present
   - Detailed responsibilities and achievements

3. **Volunteering**
   - Web Development for Dalmada Water Cooperation NGO (2023)
     - Link button to live website (https://dalmadawater.co.za/)
   - Sustainable Farming & Development Projects (2015-2018)
     - Dedicated detail page with photo gallery

4. **Core Skills**
   - 7 categories: Graphic Design, Web Dev, Office Productivity, Digital Marketing, Cloud Computing, AI & Emerging Tech, Languages
   - Skill tags with neon styling

### Projects Section
Featured work with background images and hover effects:
- Personal Portfolio Website (this site)
- NGO Website for Dalmada Water Cooperation (with background image styling)
- Azure Cloud Learning Journey

### Portfolio Preview
Links to 4 gallery categories:
- Photography (nature & wildlife)
- Logo Design
- Graphic Design & Marketing (merged marketing materials and social media)
- Product Mockups

### Contact Section
- Contact form with validation
- Email, phone, location information
- Social media links (LinkedIn, GitHub, Instagram)

## 🎯 Design System Details

### CSS Variables
```css
:root {
    --primary-color: #00ffff;      /* Neon cyan */
    --secondary-color: #ff00ff;    /* Neon magenta */
    --accent-color: #00ff88;       /* Neon green */
    --bg-dark: #0a0a0f;           /* Dark background */
    --card-bg: #12121a;           /* Card background */
    --text-color: #e0e0e0;        /* Light text */
    --text-light: #a0a0a0;        /* Muted text */
}
```

### Key Animations
- `@keyframes scanline`: Vertical moving line effect
- `@keyframes pulse`: Glowing pulse effect
- `@keyframes glitch`: Text distortion effect
- `@keyframes timeline-glow`: Pulsing timeline dots
- `@keyframes dot-pulse`: Resume timeline indicators

### Component Patterns
- **Cards**: `clip-path: polygon(15px 0, 100% 0, 100% calc(100% - 15px), calc(100% - 15px) 100%, 0 100%, 0 15px)`
- **Buttons**: Neon borders with hover glow and scale transforms
- **Timeline**: Vertical line with pulsing dots and connecting lines
- **Gallery Grid**: Responsive grid with hover overlay effects

## 📱 Responsive Design

### Breakpoints
- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px

### Mobile Optimizations
- Hamburger menu navigation
- Stacked grid layouts
- Touch-friendly button sizes
- Optimized font scaling
- Single-column project cards

## 🔧 Development Guidelines

### Adding New Portfolio Items

1. **Gallery Pages**: Follow existing pattern in `photography.html`, `logo-design.html`, etc.
   ```html
   <div class="gallery-item">
       <img src="./Images/your-image.jpg" alt="Description">
       <div class="gallery-caption">
           <h3>Title</h3>
           <p>Description</p>
       </div>
   </div>
   ```

2. **Project Cards**: Use existing structure in index.html projects section
   ```html
   <article class="project-card">
       <div class="project-image">
           <img src="Images/project.jpg" alt="Project name">
           <div class="project-overlay">
               <a href="link" class="project-link">
                   <i class="fas fa-link"></i>
               </a>
           </div>
       </div>
       <div class="project-info">
           <h3>Project Title</h3>
           <p>Description</p>
           <div class="project-tags">
               <span>Tech 1</span>
               <span>Tech 2</span>
           </div>
       </div>
   </article>
   ```

### Adding Background Images to Cards
Use inline styles for one-off customizations:
```html
<div class="project-image" style="background-image: url('Images/bg.jpg'); background-size: cover; background-position: center;">
```

### Maintaining Design Consistency
- Use CSS variables for colors
- Apply `clip-path` polygon for geometric shapes
- Include hover effects with `transform: scale()` and box-shadow glow
- Use Orbitron for headers, Rajdhani for body text
- Add appropriate Font Awesome icons

## ♿ Accessibility Features

- Semantic HTML5 elements (`<header>`, `<main>`, `<section>`, `<article>`, `<nav>`, `<footer>`)
- ARIA labels on interactive elements
- Proper heading hierarchy (h1 → h2 → h3)
- Alt text on all images
- Form labels with accessible structure
- Keyboard navigation support
- Sufficient color contrast (neon colors on dark backgrounds)
- `aria-hidden="true"` on decorative icons

## 🚀 Deployment

The site is static HTML/CSS/JS and can be deployed to:
- **GitHub Pages**: Push to repo, enable in Settings > Pages
- **Netlify**: Drag and drop folder or connect Git repo
- **Vercel**: Import from Git or upload directly
- **Traditional hosting**: FTP upload to web server

## 🔄 Recent Updates

- Merged marketing materials and social media galleries into single page
- Created separate mockups gallery page with 6 items
- Added dedicated sustainable-projects.html detail page with photo gallery
- Moved AI Prompt Engineering from Projects to Education & Skills sections
- Added background image to NGO Website project card
- Added external link button to Dalmada Water Cooperation website
- Expanded mockups gallery with placeholder images (ready for actual mockup files)

## 📝 Content Alignment

Website content is aligned with professional CV:
- Hero description matches professional summary
- Experience section structured per CV timeline
- Skills reorganized into 7 clear categories
- Education includes all degrees and certifications
- Volunteering section includes all community work

## 🎨 Customization Notes

### Replacing Placeholder Images
Several placeholder images are currently used:
- Mockups gallery: 5 items use placeholder.com URLs (t-shirt, hoodie, mug, tote bag, poster)
- Sustainable projects gallery: 6 items use via.placeholder.com URLs

Replace with actual images:
```html
<!-- Change from: -->
<img src="https://via.placeholder.com/800x600" alt="...">
<!-- To: -->
<img src="./Images/your-photo.jpg" alt="Descriptive text">
```

### Color Theme Modification
To change the color scheme, update CSS variables in `style.css`:
```css
:root {
    --primary-color: #your-color;    /* Main accent */
    --secondary-color: #your-color;  /* Secondary accent */
    --accent-color: #your-color;     /* Third accent */
}
```

All components will automatically inherit the new colors.

## 🌐 Live Features

- **Smooth scrolling** navigation
- **Mobile hamburger menu** with slide animation
- **Scroll-triggered animations** for content reveal
- **Hover effects** on all interactive elements
- **External links** open in new tabs with proper security attributes
- **Contact form** with validation (requires backend integration)

## 🐛 Known TODOs

- [ ] Replace mockup placeholder images with actual mockup files
- [ ] Replace sustainable farming gallery placeholders with real project photos
- [ ] Integrate contact form with backend service (Formspree, EmailJS, or custom)
- [ ] Add meta tags for SEO optimization
- [ ] Consider adding Open Graph tags for social media sharing

## 📞 External Links

- **Dalmada Water NGO**: https://dalmadawater.co.za/
- **GitHub**: Update with actual GitHub profile URL
- **LinkedIn**: Update with actual LinkedIn profile URL
- **Instagram**: Update with actual Instagram handle

---

**Built with passion for retro-futuristic design and modern web standards** 🚀✨
