---
description: Generates a web application using JS, HTML+CSS, Python and SQLite based on provided requirements.
---

# Detailed description
This skill is used for creating web application with Python, JS, HTML+CSS, and SQL

## Stack 
- backend: Flask + Blueprints
- frontend: HTML + CSS, Javascript
- templates: Jinja2 (built-in Flask)
- local database: SQLite (via SQLAlchemy)

## Code style
- Short and simple function names(for example: add_client)
- Add simple and clear comment above each function
- Always ask about changes you want to provide
- Keep the structure of the project clean and simple
- Divide code in different files depending on one page, so the structure of the project will be readable (EXCEPT FROM JS FILES).
- One function does one thing only
- You can edit structure with my permissions if in your opinion it will seem better.

## Project structure
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

## Frontend styles 
If plugin "frontend-design" is downloaded - follow the rules about the styles from there. If no follow the rules from this skill.

### Design Thinking (Pre-Code Phase)
Before coding, understand context and commit to a bold aesthetic direction:
- Purpose — What problem does this interface solve? Who uses it?
- Tone — Pick an extreme: brutally minimal, maximalist chaos, retro-futuristic, organic/natural, luxury/refined, playful, editorial/magazine, brutalist/raw, art deco/geometric, soft/pastel, industrial, etc.
- Constraints — Framework, performance, accessibility requirements
- Differentiation — What makes this unforgettable?

### Aesthetic Guidelines
- Typography (Choose beautiful unique fonts. Avoid generic fonts like Arial, Inter, Roboto. Pair a distinctive display font with a refined body font.)
- Color & Theme (Cohensive palette via CSS variables. Dominant colors + sharp accents>timid, evently-distributed palettes)
- Motion(CSS-only animations for HTML. Focus on high-impact moments like stagged page-load reveals, scroll triggers, surprising hover states)
- Spatial Composition (Unexpected layouts, asymmetry, overlap, diagonal flow, grid breaking elements, generous negative space OR cntrolled density)
- Backgrounds & Details (Gradient meshes, noise textures, geometric patterns, layered transparencies, dramatic shadows, decorative borders, custom cursors, grain overlays)
### NEVER USE:
- Overused fonts
- Cliched color schemes (purple gradients on white)
- Predictable layouts and cookie-cutter components
- The same design twice — vary themes, fonts, aesthetics across generations
- Convergence on common choices (e.g. Space Grotesk)
### ALWAYS
- Implement real, working code (HTML/CSS/JS, React, Vue, etc.)
- Match implementation complexity to the aesthetic vision
- Make every design visually striking, cohesive, and memorable
- Execute with intentionality — bold maximalism and refined minimalism both work

## Steps to build proper program
1. Collect requirements via the build-site skill before starting (ask about purpose, pages, database, design).
2. Based on the requirements create proper project structure.
3. Set up Flask app with Blueprints in app.py
4. Create models.py with database tables 
5. Create routes for each page
6. Create HTML templates for each page
7. Write CSS styles for each HTML template 
8. Add JavaScript in one file 
9. Test: run 'python app.py' and check for errors

## Commands
- Run app: python app.py

## Do not
- Do not add any external libraries or frameworks (no npm, no CDN) without permission
- Do not split into multiple JS files
- Do not make it complicated - simple always win
- Do not fabricate information - better say "I don't know" rather than hallucinating or lying to me. Honesty is the main tool here
- Do not use Typescript - plain Javascript only
