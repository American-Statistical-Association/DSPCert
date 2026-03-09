# DSP Certification Guidelines — Quarto Book Project

## Setup

This is a Quarto book project. To render it in RStudio:

### Prerequisites

1. Install [Quarto](https://quarto.org/docs/get-started/) (v1.3 or later recommended)
2. RStudio 2022.07 or later (has built-in Quarto support)

### Rendering

Open the project folder in RStudio, then in the Terminal run:

```bash
# Render HTML (recommended for web publishing)
quarto render

# Render PDF (requires LaTeX, e.g., TinyTeX)
quarto render --to pdf

# Preview with live reload
quarto preview
```

Or use the **Render** button in RStudio after opening any `.qmd` file.

### Project Structure

```
dsp-certification/
├── _quarto.yml          # Project config (theme, chapters, format)
├── custom.scss          # ASA brand colors and styling
├── index.qmd            # Landing/home page
└── chapters/
    ├── 01-introduction.qmd
    ├── 02-level-distinctions.qmd
    ├── 03-membership.qmd
    ├── 04-ethical-standards.qmd
    ├── 05-educational-requirements.qmd
    ├── 06-experience.qmd
    ├── 07-professional-competence.qmd
    ├── 08-professional-development.qmd
    ├── 09-application-form.qmd
    ├── 10-dssc.qmd
    ├── 11-appeals.qmd
    ├── 12-maintenance.qmd
    ├── 13-renewal.qmd
    ├── 14-other-certifications.qmd
    ├── 15-disciplinary.qmd
    ├── 16-conflict-of-interest.qmd
    ├── 17-public-information.qmd
    ├── 18-usage-of-designation.qmd
    ├── 19-dissolution.qmd
    └── appendix-1.qmd
```

### Publishing

To publish to Quarto Pub:
```bash
quarto publish quarto-pub
```

To publish to GitHub Pages:
```bash
quarto publish gh-pages
```

### Customization

- Edit `custom.scss` to change colors, fonts, or layout
- Edit `_quarto.yml` to change theme, add/remove chapters, or configure PDF output
- The `$asa-navy` and `$asa-blue` variables in `custom.scss` control the primary color scheme
