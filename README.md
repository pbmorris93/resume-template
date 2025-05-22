# LaTeX Resume Template

This repository contains a professional LaTeX-based resume template that produces a clean, ATS-friendly PDF resume.

## Overview

This template offers a modern, professional layout for your resume with:

- Clean typography and formatting
- Two-column layout options
- Section formatting with consistent styling
- ATS-friendly output
- Footer with page numbering
- Contact information with icons
- Customizable sections for experience, skills, and education

## Files

The repository includes:

- `resume-template.tex`: The main LaTeX source file (template version)
- `resume-template.pdf`: Sample PDF output

## Getting Started

### Step 1: Install LaTeX

Before using this template, ensure LaTeX is installed on your system:

#### macOS:
```bash
brew install --cask mactex
```
Or for a smaller installation:
```bash
brew install --cask basictex
```

#### Windows:
Download and install [MiKTeX](https://miktex.org/download) or [TeX Live](https://tug.org/texlive/windows.html)

#### Linux:
```bash
sudo apt-get install texlive-full
```

### Step 2: Create Your Resume

1. Make a copy of the template file by renaming `resume-template.tex` to something like `your-name-resume.tex`

2. Open the file in your preferred text editor (VS Code with LaTeX Workshop extension recommended)

3. Customize the following sections:
   - Personal information in the header
   - Experience section with your work history
   - Skills section with your technical and soft skills
   - Education section with your academic background

### Step 3: Compile Your Resume

#### Using the command line:
```bash
pdflatex your-name-resume.tex
```

#### Using VS Code:
1. Install the LaTeX Workshop extension
2. Open your `.tex` file
3. Use the "Build LaTeX project" button (or Cmd/Ctrl+Alt+B)
4. Use the "View PDF" button to see the result

## Template Structure

The template uses several custom environments:

- `\begin{header}...\end{header}`: For the resume header with your name and contact info
- `\begin{twocolentry}{right-column-text}...\end{twocolentry}`: For two-column entries (like job titles + dates)
- `\begin{onecolentry}...\end{onecolentry}`: For single-column content
- `\begin{highlights}...\end{highlights}`: For bullet point lists

## Customization Tips

- Replace placeholder text in brackets `[like this]` with your actual information
- Keep bullet points concise and achievement-focused
- For job experiences, focus on accomplishments rather than duties
- Quantify achievements where possible (percentages, metrics, etc.)
- Maintain consistent formatting throughout
- Run `pdflatex` twice if you have references or complex layouts

## Required LaTeX Packages

This template uses several LaTeX packages that might need to be installed:

```bash
tlmgr install fontawesome5 ebgaramond titlesec tabularx xcolor enumitem amsmath hyperref eso-pic calc bookmark lastpage changepage paracol ifthen needspace iftex
```

## PDF Output

The compiled PDF is designed to be both visually appealing and ATS (Applicant Tracking System) friendly.