# Quarto Web Project

A personal website built with [Quarto](https://quarto.org/). This repository hosts source files for pages such as the author bio, highlighted projects, and a resume. The site demonstrates custom styling, embedded PDFs, and various Quarto features (e.g., sections, cross-referencing, custom CSS).

## Table of Contents

- [Features](#features)
- [Repository Structure](#repository-structure)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Customization](#customization)
- [License](#license)

## Features

- **Quarto-based** website: easy to write in markdown and render to HTML.
- **Responsive custom layout**: uses a gradient background, styled sections, and CSS overrides for Quarto’s default elements.
- **Multiple Pages**:
  - **Home/About the Author**  
  - **Projects**  
  - **Resume (embedded PDF + Download Button)**
- **Navbar** integration: consistent navigation across pages (optional).
- **Custom CSS**: additional styling beyond Quarto’s defaults.

## Repository Structure

A typical layout might look like this:


- **about.qmd**: “About the Author” page.
- **projects.qmd**: “Highlighted Projects” page.
- **resume.qmd**: Resume page (with embedded PDF + Download button).
- **index.qmd**: Landing (home) page.
- **_quarto.yml**: Main configuration file for your Quarto project (site title, output format, navigation, etc.).
- **styles/**: Directory for custom CSS files.
- **assets/**: Images, PDFs, and other static files.

## Prerequisites

1. **Quarto**: Download and install the [Quarto CLI](https://quarto.org/docs/get-started/).
2. **Git**: Ensure you have [Git](https://git-scm.com/downloads) installed to clone and manage the repository.

## Getting Started

1. **Clone the Repository**:
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```
2. **Open the Project in your favorite code editor (VS Code, RStudio, PyCharm, etc.)**: 
3. **Install Quarto if you haven’t done so (see Quarto Docs)**

## Usage

### Local Preview

```bash
quarto preview
```

Quarto will open a local server in your web browser (e.g., [http://localhost:4200](http://localhost:4200)), where you can navigate between the pages.

### Rendering the Site

If you just want to render the site **without** a live preview:

```bash
quarto render
```

This compiles all `.qmd` files into HTML (by default) and places the outputs in a `_site/` folder (or another folder as specified in `_quarto.yml`).

### Deployment

- **GitHub Pages**:  
  1. Enable GitHub Pages for your repository (e.g., “main” branch and `root` folder, or use the `_site/` folder).  
  2. Push your rendered site to the appropriate branch/folder.  
  3. Go to your repository’s **Settings** > **Pages** and confirm it’s published.

- **Netlify** or **Vercel**:  
  1. Connect your repo on the chosen platform.  
  2. Configure the build command to `quarto render`.  
  3. Set the output directory to `_site`.
