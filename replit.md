# DIYSustainability - Interactive Fiction

## Overview
This is an interactive fiction story about hydroponics gardening and sustainable DIY practices. The story explores decision-making paths related to purchasing and maintaining hydroponic gardens, with themes of community sharing and sustainability.

## Project Type
- **Format**: Single-page web application
- **Language**: Vanilla HTML, CSS, and JavaScript
- **Server**: Python HTTP server

## Current State
The project is fully configured and running in the Replit environment. The interactive story is accessible via the web preview and ready for deployment. The codebase has been simplified to use clean, maintainable vanilla JavaScript instead of the original complex Twine engine.

## Project Structure
```
.
├── index.html          # Interactive story (HTML/CSS/JavaScript)
├── server.py           # Python HTTP server for serving the static site
├── .gitignore          # Python gitignore
└── replit.md           # This documentation file
```

## Recent Changes (November 13, 2025)
- Imported GitHub project to Replit
- Installed Python 3.11 for HTTP server
- Created server.py with cache control headers (prevents caching issues in iframe)
- Configured web-server workflow on port 5000
- Set up deployment configuration for autoscale
- Created project documentation
- **Simplified codebase**: Converted from Twine engine (thousands of lines with jQuery, es6-shim, Harlowe) to clean vanilla JavaScript (~250 lines)
- Preserved all story content and functionality while improving maintainability

## Technical Details

### Server Configuration
- **Host**: 0.0.0.0 (required for Replit proxy)
- **Port**: 5000 (frontend port for Replit webview)
- **Cache Control**: Disabled to ensure updates are visible immediately

### Workflow
- **Name**: web-server
- **Command**: `python server.py`
- **Output Type**: webview
- **Status**: Running

### Deployment
- **Target**: autoscale (stateless static site)
- **Run Command**: `python server.py`

## How to Use
1. The story starts at the "Log In" passage
2. Click on blue hyperlinks to make choices and navigate the story
3. Explore different paths about purchasing hydroponics equipment and gardening practices

## Story Content
The interactive fiction covers:
- Purchasing decisions (starter kits vs. full-size systems)
- Second-hand equipment options
- Plant selection (tomatoes, herbs)
- Social media integration for community support
- Sustainable gardening practices

## Development Notes
- This is a self-contained Twine project with all JavaScript and CSS embedded in the HTML file
- No build process required
- No external dependencies beyond the Python HTTP server
- The 404 error for favicon.ico is expected and does not affect functionality
