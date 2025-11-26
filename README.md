# Personal Portfolio Website

A modern, responsive personal portfolio website built with HTML, CSS, and JavaScript.

## Features

- ✨ Modern, clean design
- 📱 Fully responsive (works on desktop, tablet, mobile)
- 🎨 Professional color scheme
- 📄 CV/Resume download button
- 🔗 Social media links
- ⚡ Smooth scrolling navigation
- 🎯 SEO-friendly HTML structure

## Sections

- **Hero**: Eye-catching introduction
- **About**: Brief overview about yourself
- **Skills**: Display your technical skills
- **Projects**: Showcase your work
- **Contact**: Easy ways to get in touch

## How to Use

1. **Place your CV**: Add your `RIJUL_CV.pdf` in the root directory
2. **Update your information**:
   - Edit `index.html` to add your content
   - Update skills in the Skills section
   - Add your projects in the Projects section
   - Update social media links in the Contact section

3. **Customize colors** (optional):
   - Edit CSS variables in `styles.css` `:root` section
   - Change `--primary-color`, `--secondary-color`, etc.

## Deploying to GitHub Pages

1. Create a GitHub repository named `yourusername.github.io`
2. Push these files to your repository
3. Your site will be live at `https://yourusername.github.io`

### Steps:
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git branch -M main
git push -u origin main
```

## File Structure

```
website/
├── index.html          # Main HTML file
├── styles.css          # All styling
├── script.js           # JavaScript functionality
├── RIJUL_CV.pdf        # Your CV/Resume
├── README.md           # This file
└── .gitignore          # Git ignore file
```

## Customization Tips

- **Add more projects**: Duplicate a `.project-card` div in the Projects section
- **Change colors**: Update CSS variable values in `styles.css`
- **Add images**: Create an `images/` folder and reference images in your HTML
- **Update social links**: Change URLs in the Contact section

## Browser Support

Works on all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## License

This portfolio template is free to use and modify for your personal use.

---

Built with ❤️ using HTML, CSS & JavaScript
