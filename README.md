# hugo-mock-landing-page-autodeployed

This is a Hugo-powered static website with automated deployment to GitHub using GitHub Actions. 

# Workflow details

This workflow automatically runs on pushes to the main branch. 

1. Repository Checkout

Fetches all repository submodules
Retrieves full Git history for accurate site generation

2. Hugo Environment Setup

Initializes Hugo static site generator
Uses extended version for advanced features

3. Site Compilation

Builds static files with the following options:

Includes draft content (-D)
Applies garbage collection (--gc)
Minifies output files (--minify)

4. GitHub Pages Deployment

Publishes compiled site to gh-pages branch
Uses GitHub Actions bot for commits
