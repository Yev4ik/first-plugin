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

### Commands

| Command | Description |
|---------|-------------|
| `/build-site` | Interactive questionnaire that collects requirements (pages, database needs, design preferences) before generating a web app |

### Skills

| Skill | Description |
|-------|-------------|
| `build-website` | Generates a complete web application following the defined stack, project structure, code style, and design guidelines |
| `debug` | Diagnoses and fixes issues — routes, templates, database, auth, and frontend problems — with clear explanations |
| `review` | Reviews project structure, code quality, and UI with a scored checklist (out of 10) and actionable suggestions |

## Installation

Add this plugin to your Claude Code setup:

```bash
claude plugin add Yev4ik/first-plugin
```

Or for local development, clone the repo and add the path:

```bash
claude --plugin-dir ./first-plugin
```

## Usage

Start by running the `/build-site` command to scaffold a new web application. The plugin will ask you about your site's purpose, pages, database needs, and design preferences, then generate the project.

Use the `debug` and `review` skills naturally by describing your problem ("this route doesn't work", "review my project") and Claude will activate them automatically.
