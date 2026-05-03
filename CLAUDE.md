# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a collection of one-off web tools built as minimalist HTML applications. Each tool is completely self-contained and can be hosted on static file storage. Each tool should do one thing.

## Architecture

Each tool lives in its own directory with a single `index.html` file that contains:

- All HTML markup
- Embedded CSS in `<style>` tags
- Embedded JavaScript in `<script>` tags
- No external dependencies or build process

**No build, test, or lint commands** - These are vanilla HTML/CSS/JS files with no build tooling.

## Creating New Tools

When adding a new tool:

1. Create a new directory with a descriptive name (use kebab-case)
2. Create a single `index.html` file containing all markup, styles, and scripts. If the file gets too big, split styles and scripts into separate, single files.
3. Use vanilla JavaScript (no frameworks or external dependencies)
4. Include responsive design with mobile-friendly styles

## Code Patterns

**JavaScript**: Plain vanilla JavaScript patterns:

- DOM manipulation via `getElementById()` and `querySelector()`
- Event listeners attached directly to elements
- No external libraries or frameworks
- Audio using Web Audio API (as seen in interval-timer)

**State Management**: Keep it simple with module-level variables since each tool is self-contained and single-purpose.
