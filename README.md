# TechVision Solutions Website

![TechVision Solutions](https://img.shields.io/badge/TechVision-Solutions-blue?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## 🚀 Project Overview

TechVision Solutions is a modern, responsive website for a technology consulting firm specializing in digital transformation, cloud migration, and enterprise software solutions. The website features a stunning video background, glass-morphism design elements, and smooth animations.

## ✨ Features

### 🎨 Design & UI
- **Video Background Hero Section** - Immersive full-screen video with overlay
- **Glass-morphism Effects** - Modern frosted glass navigation and cards
- **Gradient Backgrounds** - Beautiful color transitions throughout sections
- **Responsive Design** - Optimized for all device sizes
- **Smooth Animations** - Hover effects and transitions

### 🛠️ Technical Features
- **Modern CSS Framework** - Built with Tailwind CSS
- **Custom Typography** - Google Fonts integration (Abel, Exo 2, Source Code Pro)
- **Interactive Elements** - Hover effects with color transitions
- **Semantic HTML** - Proper structure and accessibility
- **Cross-browser Compatible** - Works on all modern browsers

### 📱 Sections
- **Hero Section** - Video background with company branding
- **About Us** - Company information with gradient styling
- **Services** - Four core service offerings with interactive cards
- **Footer** - Contact information, links, and location map


## 🚀 Getting Started

### Prerequisites
- **Node.js** (v14 or higher)
- **npm** (comes with Node.js)

### Installation

1. **Clone or download the project**
   ```bash
   cd folder
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Build Tailwind CSS**
   ```bash
   npm run start
   ```
   This will watch for changes and automatically rebuild the CSS.

4. **Open the website**
   - Navigate to `HTML/index.html` in your browser
   - Or use a live server extension in your code editor

## 🛠️ Development

### Build Commands
```bash
# Watch mode (recommended for development)
npm run start

# One-time build
npx tailwindcss -i ./CSS/style.css -o ./CSS/main.css
```

### File Structure Explanation

- **`HTML/index.html`** - Main website file
- **`CSS/style.css`** - Tailwind directives (input file)
- **`CSS/main.css`** - Generated CSS (output file)
- **`tailwind.config.js`** - Tailwind configuration
- **`package.json`** - Dependencies and scripts
- **`assets/`** - All images, videos, and icons

### Key Technologies

- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first CSS framework
- **JavaScript** - Minimal custom scripts
- **Google Fonts** - Typography enhancement

## 🎨 Design System

### Color Palette
```css
/* Primary Colors */
Blue: #2563eb (bg-blue-600)
Purple: #9333ea (bg-purple-600)
Yellow: #facc15 (text-yellow-400)

/* Gradients */
Hero Background: from-blue-50 via-white to-indigo-100
Services Background: from-gray-50 via-blue-50 to-purple-50

/* Transparency */
Navbar: bg-black/10 (10% opacity)
Video Overlay: bg-black/60 (60% opacity)
```

### Typography
```css
/* Font Families */
Headings: 'Exo 2' (font-exo2)
Body Text: 'Abel' (font-abel)
Code/Tech: 'Source Code Pro' (font-source-code)
```

### Glass-morphism Effects
```css
/* Navigation */
backdrop-blur-md + bg-black/10

/* Service Cards */
bg-white/90 + backdrop-blur-sm + border-white/30
```

## 📱 Responsive Breakpoints

- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

Key responsive features:
- Flexbox layout adjustments
- Image size scaling
- Typography scaling
- Navigation adaptations

## 🎯 Performance Optimizations

- **Video Optimization** - Compressed background video
- **Image Optimization** - SVG icons for scalability
- **CSS Optimization** - Tailwind purges unused styles
- **Lazy Loading** - Video and images load efficiently

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🔧 Customization

### Changing Colors
Edit `tailwind.config.js` to modify the color scheme:
```javascript
module.exports = {
  theme: {
    extend: {
      colors: {
        'custom-blue': '#your-color',
        'custom-purple': '#your-color'
      }
    }
  }
}
```

### Adding New Sections
1. Add HTML structure in `index.html`
2. Use Tailwind classes for styling
3. Rebuild CSS with `npm run start`

### Replacing Video
1. Replace `assets/14209120-uhd_3840_2160_30fps.mp4`
2. Update the `src` attribute in the video tag
3. Ensure video is optimized for web (< 10MB recommended)

## 🚀 Deployment

### Option 1: Static Hosting
1. Build the final CSS: `npm run start`
2. Upload all files to your hosting provider
3. Ensure proper file paths are maintained

### Option 2: GitHub Pages
1. Push to GitHub repository
2. Enable GitHub Pages in repository settings
3. Set source to root directory

### Option 3: Netlify/Vercel
1. Connect repository
2. Set build command: `npm run start`
3. Set publish directory: `/`

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👥 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request



## 🛠️ Technical Notes

### Tailwind Configuration
The project uses custom content paths:
```javascript
content: [
  "./HTML/**/*.html",
  "./CSS/**/*.css",
  "./**/*.js",
]
```

### Video Background Setup
```html
<!-- Hero container with relative positioning -->
<div class="hero-container h-[100vh] overflow-hidden">
  <!-- Absolute positioned video -->
  <video class="absolute top-0 left-0 w-full h-full object-cover">
    <source src="../assets/video.mp4" type="video/mp4">
  </video>
  <!-- Dark overlay for text readability -->
  <div class="absolute top-0 left-0 w-full h-full bg-black/60"></div>
</div>
```

### Glass Effect Implementation
```html
<!-- Navigation with glass effect -->
<nav class="backdrop-blur-md bg-black/10">
  <!-- Content -->
</nav>

<!-- Service cards with glass effect -->
<div class="bg-white/90 backdrop-blur-sm border border-white/30">
  <!-- Content -->
</div>
```

---

**Built with ❤️ by [Prakshil Patel]**
