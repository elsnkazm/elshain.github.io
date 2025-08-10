<<<<<<< HEAD
# Elshain Website

A modern, responsive website for Elshain built with HTML, CSS, and JavaScript, designed to be deployed on GitHub Pages.

## Features

- **Responsive Design**: Mobile-first approach with modern CSS Grid and Flexbox
- **Modern UI**: Clean, professional design with smooth animations
- **SEO Optimized**: Proper meta tags, structured data, and semantic HTML
- **Fast Loading**: Optimized assets and minimal dependencies
- **Accessible**: WCAG compliant with proper ARIA labels and keyboard navigation

## Tech Stack

- **HTML5**: Semantic markup with modern features
- **CSS3**: Custom properties, Grid, Flexbox, and animations
- **JavaScript**: Vanilla JS with modern ES6+ features
- **GitHub Pages**: Free hosting with custom domain support

## Getting Started

### Prerequisites

- A GitHub account
- A domain name (elshain.com)
- Basic knowledge of Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/elshain/elshain.github.io.git
   cd elshain.github.io
   ```

2. **Customize the content**
   - Edit `index.html` to update your content
   - Modify `styles.css` to change the design
   - Update contact information and links

3. **Test locally**
   - Open `index.html` in your browser
   - Test responsive design on different screen sizes
   - Verify all links and forms work correctly

### Deployment

1. **Push to GitHub**
   ```bash
   git add .
   git commit -m "Initial website setup"
   git push origin main
   ```

2. **Configure GitHub Pages**
   - Go to your repository settings
   - Navigate to "Pages" section
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Save the settings

3. **Set up custom domain**
   - In the Pages settings, enter "elshain.com" in the custom domain field
   - Check "Enforce HTTPS"
   - Save the settings

4. **Configure DNS**
   Add these records to your domain registrar:
   ```
   Type: A
   Name: @
   Value: 185.199.108.153
   Value: 185.199.109.153
   Value: 185.199.110.153
   Value: 185.199.111.153
   
   Type: CNAME
   Name: www
   Value: elshain.github.io
   ```

## File Structure

```
elshain.github.io/
├── index.html          # Main homepage
├── styles.css          # Stylesheet
├── script.js           # JavaScript functionality
├── CNAME               # Custom domain configuration
├── _config.yml         # Jekyll configuration
├── .gitignore          # Git ignore rules
├── README.md           # Project documentation
├── robots.txt          # SEO configuration
├── sitemap.xml         # XML sitemap
└── favicon.ico         # Website favicon
```

## Customization

### Colors
The website uses CSS custom properties for easy color customization. Edit the root variables in `styles.css`:

```css
:root {
  --primary-color: #3b82f6;
  --secondary-color: #64748b;
  --background-color: #ffffff;
  --text-color: #1e293b;
}
```

### Content
- Update the hero section text in `index.html`
- Modify service descriptions and contact information
- Replace placeholder images with your own assets

### Styling
- Edit `styles.css` to change fonts, spacing, and layout
- Modify animations and transitions
- Adjust responsive breakpoints

## SEO Features

- Semantic HTML structure
- Meta tags for social media sharing
- Open Graph and Twitter Card support
- XML sitemap
- Robots.txt configuration
- Fast loading times
- Mobile-friendly design

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

- Email: contact@elshain.com
- Website: https://elshain.com

## Acknowledgments

- [Inter Font](https://rsms.me/inter/) for typography
- [Feather Icons](https://feathericons.com/) for SVG icons
- [GitHub Pages](https://pages.github.com/) for hosting 
=======
# elshain.github.io
>>>>>>> c3f72b02ebd21dd32cee18d424dc91d58f1cca8f
