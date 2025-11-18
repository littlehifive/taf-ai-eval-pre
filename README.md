# AI Evaluation Playbook Presentation

This folder contains the R Markdown presentation based on the Generative AI Evaluation in the Development Sector playbook.

## Files

- `ai_eval_presentation.Rmd` - The main R Markdown source file
- `ai_eval_presentation.html` - HTML presentation (ioslides format) with modern styling
- `ai_eval_presentation.pptx` - PowerPoint presentation
- `styles.css` - Custom CSS styling for the HTML presentation (includes Google Fonts, gradients, improved typography)

## Styling Improvements

### HTML Presentation
- **Modern Design**: Gradient title slide with purple/blue theme (#667eea to #764ba2)
- **Typography**: Inter font family for clean, professional look
- **Fixed Lists**: Bullet points now render properly with correct spacing and indentation
- **Enhanced Tables**: Gradient headers, hover effects, rounded corners
- **Better Spacing**: Improved margins, padding, and line heights for readability
- **Color Scheme**: Professional blue/purple gradient theme throughout

### PowerPoint Presentation
- Uses default Office theme (PowerPoint templates require manual creation of .pptx template files)
- Content is well-structured and formatted
- To customize further, create a PowerPoint template (.pptx) with custom layouts and reference it in the YAML: `reference_doc: template.pptx`

## Regenerating Presentations

To regenerate the presentations, you can use R or RStudio:

### From R Console:

```r
library(rmarkdown)

# Generate HTML presentation
render('ai_eval_presentation.Rmd', output_format = 'ioslides_presentation')

# Generate PowerPoint presentation
render('ai_eval_presentation.Rmd', output_format = 'powerpoint_presentation')
```

### From Command Line:

```bash
# HTML
Rscript -e "library(rmarkdown); render('ai_eval_presentation.Rmd', output_format = 'ioslides_presentation')"

# PowerPoint
Rscript -e "library(rmarkdown); render('ai_eval_presentation.Rmd', output_format = 'powerpoint_presentation')"
```

## Requirements

- R (with rmarkdown package)
- Pandoc 2.0.5 or higher (for PowerPoint output)
- For PowerPoint: Microsoft PowerPoint or compatible software to view/edit

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

