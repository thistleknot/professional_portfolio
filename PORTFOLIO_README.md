# Professional Portfolio Website

A clean, professional portfolio website built with [HugoBlox](https://hugoblox.com/) and hosted on GitHub Pages.

## ✨ Features

- **Professional Resume Theme** — Clean, minimal design with built-in dark mode
- **Portfolio Sections:**
  - About/Bio with profile image
  - Resume/Experience with work history and education
  - Side Projects showcase (3+ projects)
  - Work Projects with business impact metrics
  - Skills and languages
- **Fully Customizable** — All content is Markdown — easy to edit and version control
- **No Lock-In** — Your content is plain text files, yours to keep forever
- **SEO Optimized** — Built-in sitemap, structured data, and search engine optimization
- **Responsive Design** — Looks great on mobile, tablet, and desktop
- **Auto Dark Mode** — Automatically adapts to system preferences

## 📁 Project Structure

```
portfolio/
├── content/
│   ├── authors/me/            # Your profile information
│   ├── projects/
│   │   ├── side-projects/     # Your personal projects (3 templates)
│   │   └── work-projects/     # Your professional work (3 templates with business impact)
│   └── _index.md              # Home page combining all sections
├── config/
│   ├── hugo.yaml              # Site configuration
│   ├── params.yaml            # Portfolio settings
│   └── ...
├── static/
│   └── uploads/resume.pdf     # Your resume file
├── assets/
│   ├── media/                 # Images for projects
│   └── authors/me/            # Your profile picture
├── PORTFOLIO_GUIDE.md         # Detailed content editing guide
├── GITHUB_PAGES_DEPLOY.md     # Deployment instructions
└── README.md                  # This file
```

## 🚀 Quick Start

### 1. Local Setup
Your portfolio is already set up locally at:
```
C:\Users\user\Documents\dev\profile
```

The boilerplate includes:
- ✅ 3 sample side projects
- ✅ 3 sample work projects with business impact templates
- ✅ Professional resume section template
- ✅ Skills, education, and experience sections

### 2. Update Your Information

Edit `content/authors/me/_index.md` with:
- Your name, professional title, bio
- Work history and education
- Skills and languages
- Social media links

See `PORTFOLIO_GUIDE.md` for detailed instructions.

### 3. Add Your Projects

**Side Projects** → Edit or create files in:
```
content/projects/side-projects/project-1/index.md
content/projects/side-projects/project-2/index.md
content/projects/side-projects/project-3/index.md
```

**Work Projects** → Edit or create files in:
```
content/projects/work-projects/work-project-1/index.md
content/projects/work-projects/work-project-2/index.md
content/projects/work-projects/work-project-3/index.md
```

Focus on business impact:
- Revenue generated or saved
- Performance improvements (with %)
- Scale (users, transactions, data volume)
- Team collaboration or leadership

### 4. Deploy to GitHub Pages

See `GITHUB_PAGES_DEPLOY.md` for step-by-step instructions.

In summary:
1. Create a GitHub repo named `yourusername.github.io`
2. Push your local code to GitHub
3. Enable GitHub Pages in repository settings
4. Your site goes live at `https://yourusername.github.io`

## 📚 Documentation

- **[PORTFOLIO_GUIDE.md](./PORTFOLIO_GUIDE.md)** — Comprehensive guide to updating content
  - How to edit your profile
  - How to add/update projects
  - Customization options
  - Image guidelines

- **[GITHUB_PAGES_DEPLOY.md](./GITHUB_PAGES_DEPLOY.md)** — Deployment guide
  - Step-by-step GitHub Pages setup
  - How to push updates
  - Troubleshooting

- **[Official HugoBlox Docs](https://docs.hugoblox.com/)** — Advanced customization

## 🎨 Customization

### Change Site Title & URL
Edit `config/hugo.yaml`:
```yaml
title: 'Your Portfolio Title'
baseURL: 'https://yourusername.github.io/'
```

### Change Colors
Edit `config/params.yaml`:
```yaml
hugoblox:
  theme:
    colors:
      primary: "blue"
      secondary: "purple"
```

Available colors: slate, gray, zinc, neutral, stone, red, orange, amber, yellow, lime, green, emerald, teal, cyan, blue, indigo, violet, purple, fuchsia, pink, rose

### More Customization
See `PORTFOLIO_GUIDE.md` → "Customizing Your Portfolio" section

## 📝 Content Files Included

### Resume/Profile
- `content/authors/me/_index.md` — Your main profile with education and work history

### Side Projects (3 templates)
- `content/projects/side-projects/project-1/index.md`
- `content/projects/side-projects/project-2/index.md`
- `content/projects/side-projects/project-3/index.md`

### Work Projects (3 templates)
- `content/projects/work-projects/work-project-1/index.md`
- `content/projects/work-projects/work-project-2/index.md`
- `content/projects/work-projects/work-project-3/index.md`

### Home Page
- `content/_index.md` — Combines all sections into your homepage

## 🔑 Key Features

### Work Project Best Practices

✓ Do:
- Use generic descriptions to protect confidentiality
- Include quantifiable metrics ($, %, performance gains)
- Highlight your specific contributions
- List technologies and methodologies

✗ Don't:
- Disclose confidential algorithms or proprietary logic
- Use specific company names (unless permitted)
- Include internal team structures
- Share sensitive business details

### Example Work Project
```
Title: "Payment Platform Scaling"
Business Impact:
- $2.3M annual cost reduction
- 40% latency improvement
- 3x capacity increase
- 99.99% uptime

Your Contributions:
- Designed database sharding strategy
- Led microservices migration
- Reduced average query time from 2.5s to 150ms
```

## 📦 What's Included

This boilerplate includes:
- ✅ HugoBlox theme (MIT licensed)
- ✅ Resume template pre-configured
- ✅ 3 side project templates
- ✅ 3 work project templates with business impact focus
- ✅ Git repository initialized
- ✅ Markdown-based content (future-proof)
- ✅ Config files ready to customize

## 🛠 Tech Stack

- **Hugo** — Static site generator
- **HugoBlox** — Professional website framework
- **Tailwind CSS** — Modern styling
- **GitHub Pages** — Free hosting

## 📋 Next Steps

1. **Read** `PORTFOLIO_GUIDE.md` to understand content structure
2. **Update** `content/authors/me/_index.md` with your information
3. **Edit** the 3 side projects with your real projects
4. **Edit** the 3 work projects highlighting business impact
5. **Follow** `GITHUB_PAGES_DEPLOY.md` to publish
6. **Share** your portfolio URL: `https://yourusername.github.io`

## 🔗 Useful Links

- **HugoBlox Documentation:** https://docs.hugoblox.com/
- **Hugo Documentation:** https://gohugo.io/documentation/
- **GitHub Pages Guide:** https://docs.github.com/en/pages
- **HugoBlox Discord:** https://discord.gg/z8wNYzb
- **Tailwind Colors:** https://tailwindcss.com/docs/customizing-colors

## 📄 License

This portfolio template uses HugoBlox which is licensed under MIT. See LICENSE.md for details.

---

**Ready to get started?** 

1. Start with `PORTFOLIO_GUIDE.md` for content editing
2. Then follow `GITHUB_PAGES_DEPLOY.md` to go live
3. Customize colors and settings as needed

Good luck with your portfolio! 🎉
