# AI Evaluation Playbook Presentation

This repository contains the R Markdown presentation based on the Generative AI Evaluation in the Development Sector playbook.

## Files

- `presentation/ai_eval_presentation.Rmd` - The main R Markdown source file
- `presentation/ai_eval_presentation.html` - HTML presentation (ioslides format) with modern styling
- `presentation/styles.css` - Custom CSS styling for the HTML presentation (includes Google Fonts, gradients, improved typography)
- `presentation/images/` - Image assets for the presentation

## GitHub Pages Deployment

This repository is set up with **GitHub Actions** to automatically build and deploy the presentation to GitHub Pages.

### Automatic Deployment

Every time you push changes to the `main` branch:
1. GitHub Actions automatically renders the R Markdown file to HTML
2. The HTML is deployed to GitHub Pages
3. Your presentation is live at: `https://yourusername.github.io/repo-name/`

### Setup Instructions

1. **Enable GitHub Pages:**
   - Go to your repository Settings → Pages
   - Under "Source", select "GitHub Actions"
   - Save

2. **Push your changes:**
   - The workflow will run automatically on every push to `main`
   - Check the Actions tab to see the build status

3. **Access your presentation:**
   - After the first successful deployment, your presentation will be available at your GitHub Pages URL

For more details, see `presentation/GITHUB_PAGES_SETUP.md`.

## Styling Improvements

### HTML Presentation
- **Modern Design**: Clean white background with blue accent theme (#667eea)
- **Typography**: Inter font family for clean, professional look
- **Fixed Lists**: Bullet points now render properly with correct spacing and indentation
- **Enhanced Tables**: Gradient headers, hover effects, rounded corners
- **Better Spacing**: Improved margins, padding, and line heights for readability
- **Color Scheme**: Professional blue/purple gradient theme throughout

## Regenerating Presentations Locally

To regenerate the presentations locally, you can use R or RStudio:

### From R Console:

```r
library(rmarkdown)

# Generate HTML presentation
render('presentation/ai_eval_presentation.Rmd', output_format = 'ioslides_presentation')

# Generate PowerPoint presentation (if needed)
render('presentation/ai_eval_presentation.Rmd', output_format = 'powerpoint_presentation')
```

### From Command Line:

```bash
# HTML
Rscript -e "library(rmarkdown); render('presentation/ai_eval_presentation.Rmd', output_format = 'ioslides_presentation')"

# PowerPoint (if needed)
Rscript -e "library(rmarkdown); render('presentation/ai_eval_presentation.Rmd', output_format = 'powerpoint_presentation')"
```

**Note:** The HTML presentation is automatically regenerated and deployed via GitHub Actions when you push changes, so you typically don't need to regenerate it manually.

## Requirements

### For Local Development:
- R (with rmarkdown package)
- Pandoc 2.0.5 or higher (for PowerPoint output)
- For PowerPoint: Microsoft PowerPoint or compatible software to view/edit

### For GitHub Actions:
- No local setup required! The GitHub Actions workflow automatically installs R and all dependencies.

## Content

The presentation covers:

1. **Introduction** - The challenge and four-level framework
2. **Building Blocks** - User funnels, ETL pipelines, hypotheses, experiments
3. **Cross-Functional Teams** - Roles and best practices
4. **Level 1: Model Evaluation** - Does the AI model produce desired responses?
5. **Level 2: Product Evaluation** - Does the product facilitate meaningful interactions?
6. **Level 3: User Evaluation** - Does the product support users' thoughts, feelings, knowledge, behaviors?
7. **Level 4: Impact Evaluation** - Does access improve development outcomes?

The content is faithful to the original playbook while adapted for slide format.

