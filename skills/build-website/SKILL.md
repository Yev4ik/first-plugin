---
name: build-website
description: Use when the user asks to "build a website", "create a web app", "generate a Flask project", "scaffold a site", or "make a web application". Generates a complete Flask + HTML/CSS + SQLite web application from requirements.
---

# Build Website

Generate a complete web application with Python, JS, HTML+CSS, and SQLite.

## Stack
- Backend: Flask + Blueprints
- Frontend: HTML + CSS, Javascript
- Templates: Jinja2 (built-in Flask)
- Database: SQLite (via SQLAlchemy)

## Code Style
- Use short and simple function names (e.g., `add_client`)
- Add a simple and clear comment above each function
- Always ask the user about changes before implementing them
- Keep the project structure clean and simple
- Divide code into different files per page for readability (except JS files)
- One function does one thing only
- Edit structure only with user permission

## Project Structure
```
README.md
requirements.txt
app.py
models.py
instance/
  app.db
routes/
  <page_name>.py
templates/
  <page_name>.html
static/
  css/
    <page_name>.css
  js/
    app.js
  images/
```

## Frontend Styles
If the `frontend-design` plugin is installed, follow its style rules. Otherwise follow the rules below.

### Design Thinking (Pre-Code Phase)
Before coding, understand context and commit to a bold aesthetic direction:
- Purpose — What problem does this interface solve? Who uses it?
- Tone — Pick an extreme: brutally minimal, maximalist chaos, retro-futuristic, organic/natural, luxury/refined, playful, editorial/magazine, brutalist/raw, art deco/geometric, soft/pastel, industrial, etc.
- Constraints — Framework, performance, accessibility requirements
- Differentiation — What makes this unforgettable?

### Aesthetic Guidelines
- Typography: Choose beautiful unique fonts. Avoid generic fonts like Arial, Inter, Roboto. Pair a distinctive display font with a refined body font.
- Color & Theme: Cohesive palette via CSS variables. Dominant colors + sharp accents over timid, evenly-distributed palettes.
- Motion: CSS-only animations for HTML. Focus on high-impact moments like staggered page-load reveals, scroll triggers, surprising hover states.
- Spatial Composition: Unexpected layouts, asymmetry, overlap, diagonal flow, grid-breaking elements, generous negative space OR controlled density.
- Backgrounds & Details: Gradient meshes, noise textures, geometric patterns, layered transparencies, dramatic shadows, decorative borders, custom cursors, grain overlays.

### Avoid
- Overused fonts
- Cliched color schemes (purple gradients on white)
- Predictable layouts and cookie-cutter components
- The same design twice — vary themes, fonts, aesthetics across generations

### Always
- Implement real, working code (HTML/CSS/JS)
- Match implementation complexity to the aesthetic vision
- Make every design visually striking, cohesive, and memorable

## Build Steps
1. Collect requirements via the `build-site` command
2. Create proper project structure
3. Set up Flask app with Blueprints in app.py
4. Create models.py with database tables
5. Create routes for each page
6. Create HTML templates for each page
7. Write CSS styles for each HTML template
8. Add JavaScript in one file
9. Test: run `python app.py` and check for errors

## Run Command
```
python app.py
```

## Restrictions
- Do not add external libraries or frameworks (no npm, no CDN) without user permission
- Do not split into multiple JS files
- Keep it simple — simplicity always wins
- Use plain Javascript only, no Typescript
