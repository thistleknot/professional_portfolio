# Portfolio Website Content Guide

## Overview
This is a HugoBlox-based professional portfolio website template. It includes sections for your resume, side projects, and work projects with business impact metrics.

## Structure

```
content/
├── authors/
│   └── me/
│       └── _index.md          # Your main profile information
├── projects/
│   ├── side-projects/         # Your personal/side projects
│   │   ├── project-1/index.md
│   │   ├── project-2/index.md
│   │   └── project-3/index.md
│   └── work-projects/         # Your professional work projects
│       ├── work-project-1/index.md
│       ├── work-project-2/index.md
│       └── work-project-3/index.md
├── _index.md                  # Home page with portfolio sections
uploads/
└── resume.pdf                 # Your PDF resume
```

## Updating Your Profile

### 1. Profile Information
**File:** `content/authors/me/_index.md`

Update the following fields:
- `title`: Your name
- `role`: Your professional title/headline
- `bio`: Professional biography (2-3 sentences)
- `interests`: List your key interests (3-5 items)
- `social`: Add your social media links (LinkedIn, GitHub, Twitter, etc.)
- `organizations`: Your current employer(s)
- `education`: Your degrees and certifications
- `work`: Your professional experience (listed in reverse chronological order)
- `skills`: Technical and professional skills
- `languages`: Languages you speak with proficiency levels

**Avatar Image:**
- Place your headshot at: `assets/media/authors/me/avatar.jpg` or `avatar.png`
- Recommended: 300x300px, square format

### 2. Resume File
- Place your PDF resume at: `static/uploads/resume.pdf`
- Update the button URL in `content/_index.md` if using a different filename

## Side Projects

### Adding a New Side Project

1. Create a new folder: `content/projects/side-projects/project-name/`
2. Create `index.md` file with this structure:

```yaml
---
title: "Project Name"
date: 2025-05-01              # Date (YYYY-MM-DD)
external_link: "https://github.com/yourusername/project"
image:
  filename: "project.png"     # Place image in this folder
  preview_only: false
summary: "One sentence description of your project"
tags:
  - technology1
  - technology2
---

## Overview
Detailed description of the project

## Links
- [GitHub Repository](https://github.com/yourusername/project)
- [Live Demo](https://project-demo.com)
```

3. Add a project image: Place your project image in `content/projects/side-projects/project-name/project.png`

### Key Fields:
- **title**: Project name
- **date**: When you created/published it
- **external_link**: Link to GitHub repo or live demo (appears as a button)
- **summary**: One-line description (appears in preview)
- **tags**: Used for filtering projects on the main page
- **Content**: Full project description with details about what it does, technologies used, and why you built it

## Work Projects

### Adding a New Work Project

1. Create a new folder: `content/projects/work-projects/project-name/`
2. Create `index.md` file with this structure:

```yaml
---
title: "Project Name"
date: 2024-12-01
image:
  filename: "project.png"
  preview_only: false
summary: "Generic description focusing on business value"
tags:
  - business-impact
  - technology-category
---

## Project Overview
- **Industry/Domain:** [Your industry]
- **My Role:** [Your title/role]
- **Timeline:** [Duration]

## Business Impact
- **Revenue Impact:** $X increase / X% growth
- **Cost Savings:** $X in efficiency
- **User Growth:** X% increase
- **Performance:** X% improvement

## Key Contributions
- Achievement 1 with quantified result
- Achievement 2 with quantified result
- Achievement 3 with quantified result

## Technologies Used
- Tech 1
- Tech 2
- Tech 3

## Outcome
Quantified results and lessons learned
```

### Guidelines for Work Projects:
✓ **DO:**
- Use generic industry/role descriptions
- Focus on business outcomes with numbers ($, %, growth metrics)
- Highlight your specific contributions
- List the technologies/platforms used
- Include before/after metrics

✗ **DON'T:**
- Disclose confidential client information
- Reveal proprietary algorithms or business logic
- Use specific company names (unless permitted)
- Share internal team structures or salary information

### Example Work Project:
```
Title: "Payment Processing Platform Optimization"
Business Impact:
- $2.3M annual cost reduction through infrastructure optimization
- 40% reduction in transaction processing latency
- 3x capacity increase supporting 500K+ daily transactions
- 99.99% uptime achieved

My Contributions:
- Architected database sharding strategy
- Led migration of legacy system to microservices
- Reduced query time from 2.5s to 150ms average
```

## Customizing Your Portfolio

### Config Updates

**File:** `config/hugo.yaml`
```yaml
title: 'Your Portfolio Title'
baseURL: 'https://yourusername.github.io/'  # Change 'yourusername'
```

**File:** `config/params.yaml`
- Update `identity.name` to your name
- Update `identity.tagline` with your professional headline
- Update `identity.description` with a brief bio
- Update `social.twitter` with your handle (optional)

### Site Colors
Edit `config/params.yaml` under `theme.colors`:
```yaml
colors:
  primary: "blue"        # or hex like "#3b82f6"
  secondary: "purple"
  neutral: "gray"
```

Available color names: slate, gray, zinc, neutral, stone, red, orange, amber, yellow, lime, green, emerald, teal, cyan, blue, indigo, violet, purple, fuchsia, pink, rose

## Project Images

### Side Project Images
- Location: `content/projects/side-projects/[project-name]/[project-name].png`
- Size: 400x300px or similar aspect ratio
- Format: PNG or JPG

### Work Project Images
- Location: `content/projects/work-projects/[project-name]/[project-name].png`
- Size: 400x300px or similar aspect ratio
- Format: PNG or JPG (screenshots, diagrams, or generic project visuals)

## Adding More Content

### Add Another Side Project
1. Duplicate an existing side project folder
2. Rename it to your new project name
3. Update the `index.md` file with new content
4. Add a new project image

### Add Another Work Project
1. Duplicate an existing work project folder
2. Rename it to your new project name
3. Update the `index.md` file with new content
4. Add a project image

### Change Number of Projects Displayed
Edit `content/_index.md` and look for the portfolio blocks. You can add more project folders and they'll automatically appear.

## Publishing to GitHub Pages

### Prerequisites
- GitHub account
- Git installed

### Setup Steps

1. **Create GitHub Repository**
   - Go to github.com/new
   - Repository name: `yourusername.github.io`
   - Make it **Public**
   - Click "Create repository"

2. **Initialize and Push**
   ```bash
   cd /path/to/profile
   git init
   git add .
   git commit -m "Initial portfolio commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to Settings → Pages
   - Source: Deploy from branch
   - Branch: main, folder: / (root)
   - Save

4. **Access Your Portfolio**
   - Wait 1-2 minutes for deployment
   - Visit: `https://yourusername.github.io`

### Updating Your Portfolio

After making changes:
```bash
git add .
git commit -m "Update portfolio content"
git push
```

Your site will automatically rebuild and update within a few minutes.

## Support & Resources

- **HugoBlox Documentation:** https://docs.hugoblox.com/
- **Hugo Documentation:** https://gohugo.io/documentation/
- **HugoBlox Discord:** https://discord.gg/z8wNYzb

## Tips for Great Content

1. **Resume Bio**: 2-3 sentences explaining your expertise and interests
2. **Side Projects**: Show your diverse technical interests and learning
3. **Work Projects**: Quantify everything (% improvement, $ value, scale)
4. **Consistency**: Keep tone professional but personable
5. **Completeness**: Update regularly and remove old/irrelevant content
6. **Images**: High-quality images make projects stand out more

---

Ready to deploy? Follow the "Publishing to GitHub Pages" section above!
