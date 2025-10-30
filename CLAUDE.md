# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains a professional HTML estimate for Donald McLaughlin's skylight replacement project at 170 Spalding Creek Court, Atlanta, GA 30350. The estimate is a single-page HTML document designed for GitHub Pages deployment.

## Architecture

**Single-File HTML Structure**: The entire estimate is contained in `McLaughlin_Skylight_Estimate.html` - a self-contained HTML file with embedded CSS (no external dependencies).

**Key Sections**:
- Header with SIG Skylights logo and company information
- Customer information and project description
- Detailed scope of work with 7 categories (Site Preparation, Removal, Custom Fabrication, Installation, Weatherproofing, Quality Control, Cleanup)
- Special considerations section for insurance justification
- Itemized estimate breakdown table (total: $28,569.00)
- Photo documentation grid with 29 embedded CompanyCam URLs
- Terms and conditions
- Footer

**Photo Integration**: All photos use CompanyCam CDN URLs (https://img.companycam.com/*). Photos are displayed in a responsive grid layout that adapts to different screen sizes.

**Design System**:
- Color scheme: Blue gradient (#1e3c72 to #2a5298) for headers and accents
- Responsive design with mobile breakpoints at 768px
- Print-friendly CSS media queries included
- Grid-based photo layout (auto-fill, minmax 300px)

## Deployment

**GitHub Pages**: The estimate is deployed at:
- Live URL: https://kapptech88.github.io/Donald_Mclaughlin_Skylights/McLaughlin_Skylight_Estimate.html
- Repository: https://github.com/KappTech88/Donald_Mclaughlin_Skylights

**Git Configuration**:
- Branch: `main`
- Remote: Uses personal access token authentication (token embedded in remote URL)
- User: KappTech88 (kapptech88@example.com)

## Common Updates

**Changing Estimate Date**: Update line 323 in the estimate-title section.

**Modifying Line Items**: Edit the items-table tbody section (lines 434-473). Total is manually calculated.

**Updating Photos**: Photo grid starts at line 480. Each photo-item div contains an img tag with CompanyCam URL.

**Scope of Work Changes**: The scope of work section (lines 343-421) contains detailed bullet points for insurance justification. This is a critical section for claim approval.

**Removing Content**: When removing email addresses, section titles, or captions, ensure the surrounding HTML structure remains intact (no orphaned tags).

## Deployment Workflow

To deploy changes:
```bash
git add McLaughlin_Skylight_Estimate.html
git commit -m "Description of changes"
git push origin main
```

GitHub Pages will automatically rebuild (typically within 1-2 minutes).

## Important Notes

- The estimate file has NO email addresses (removed per client request)
- Photo captions and section titles have been removed - photos appear in a single continuous grid
- The scope of work section was added specifically to justify the $28K cost for insurance adjuster approval
- Date was changed from October 30 to October 15, 2025 per client request
