# Yan Luiz - CV Portfolio Website

A simple, elegant static website to present your CV with multi-language support and download functionality.

## Features

- **Multi-language Support**: Switch between English, Portuguese (ptBR), and Spanish
- **Download Options**: Export your CV in Markdown, PDF, or DOCX format
- **Mobile Responsive**: Optimized for all device sizes
- **LLM SEO Optimized**: Includes structured data and llms.txt for LLM-based search engines
- **Clean Design**: Professional and easy-to-read layout

## Files Structure

```
docs/
├── index.html      # Main HTML file with semantic markup and SEO meta tags
├── styles.css      # Responsive CSS styling
├── script.js       # JavaScript for language switching and downloads
├── llms.txt        # LLM Search Engine Optimization file
└── README.md       # This file
```

## How to Use

### Local Development

1. Open `index.html` in your web browser
2. Or use a simple HTTP server:
   ```bash
   cd docs
   python -m http.server 8000
   ```
3. Visit `http://localhost:8000`

### GitHub Pages Deployment

1. Push this repository to GitHub
2. Go to repository Settings → Pages
3. Set source to "Deploy from a branch"
4. Select branch: `main` and folder: `/docs`
5. Save and wait for deployment
6. Your site will be available at: `https://[username].github.io/[repository]/`

### Customization

To update the CV content:

1. Edit the `cvContent` object in `script.js`
2. Update all three language versions (en, pt, es)
3. The content uses Markdown format which is automatically converted to HTML

### Language Support

The site automatically loads in English by default. Users can switch between:
- **English** (en)
- **Português** (pt)
- **Español** (es)

### Download Functionality

The download button offers three formats:
- **Markdown (.md)**: Direct markdown file download
- **PDF (.pdf)**: Generated using html2pdf.js library
- **Word (.docx)**: Generated using docx library

The downloaded file will be in the currently selected language.

## Technologies Used

- Pure HTML5, CSS3, and JavaScript (no frameworks)
- [html2pdf.js](https://github.com/eKoopmans/html2pdf.js) for PDF generation
- [docx](https://www.npmjs.com/package/docx) for Word document generation
- [FileSaver.js](https://github.com/eligrey/FileSaver.js) for file downloads

## SEO & LLM Optimization

The site includes:
- OpenGraph meta tags for social media
- Schema.org structured data for search engines
- Custom LLM meta tags for AI-based search
- llms.txt file with structured information for LLM crawlers
- Mobile-friendly viewport settings

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

This is a personal CV website. Feel free to use the structure and code for your own CV.

---

**Contact:** yan@nomadbitcoin.xyz
**GitHub:** [@nomadbitcoin](https://github.com/nomadbitcoin)
