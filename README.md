# first-plugin

A Claude Code plugin for generating web applications using Flask, HTML+CSS, JavaScript, and SQLite.

## Author

Zembytska Yeva

## What it does

This plugin helps you build, debug, and review full-stack web applications with a guided workflow. It enforces a clean project structure, bold visual design, and simple code style.

### Tech stack

- **Backend:** Flask + Blueprints
- **Frontend:** HTML + CSS + vanilla JavaScript
- **Templates:** Jinja2
- **Database:** SQLite (via SQLAlchemy)

## Components

### Skills

| Skill | Invocation | Description |
|-------|-----------|-------------|
| `build-site` | `/first-plugin:build-site` | Interactive questionnaire that collects requirements (pages, database needs, design preferences) before generating a web app |
| `build-website` | auto-invoked | Generates a complete web application following the defined stack, project structure, code style, and design guidelines |
| `debug` | auto-invoked | Diagnoses and fixes issues — routes, templates, database, auth, and frontend problems — with clear explanations |
| `review` | auto-invoked | Reviews project structure, code quality, and UI with a scored checklist (out of 10) and actionable suggestions |

## Installation

### As a plugin (recommended)

```bash
claude plugin add github:Yev4ik/first-plugin
```

### Via marketplace

```bash
/plugin marketplace add Yev4ik/first-plugin
/plugin install first-plugin@yeva-marketplace
```

## Usage

Start by running the `/first-plugin:build-site` skill to scaffold a new web application. The plugin will ask you about your site's purpose, pages, database needs, and design preferences, then generate the project.

Use the `debug` and `review` skills naturally by describing your problem ("this route doesn't work", "review my project") and Claude will activate them automatically.
