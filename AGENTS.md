# Agent Instructions & Workflow

This document outlines the rules and procedures for AI agents operating in this repository. The goal is to ensure code quality, consistency, and prevent errors.

## Core Principles
1.  **Preview Everything:** All changes must be pushed to a `preview-updates` branch first. No direct commits to `master`.
2.  **Clarity Over Brevity:** Code and commit messages should be clear and easy to understand.
3.  **User Confirmation:** Do not merge the preview branch into `master` without explicit confirmation from the user.

## Pre-Commit Checklist
Before every commit, the agent MUST perform the following checks:

- **[ ] HTML Validation:**
    - Are all HTML tags properly closed?
    - Is the document structure valid (e.g., no `<div>` inside a `<p>`)?
    - Are all `<img>` tags complete with descriptive `alt` attributes?

- **[ ] Link Verification:**
    - Do all internal links point to the correct pages (e.g., `index.html`, `contact.html`)?
    - Do all external links have `target="_blank"`?

- **[ ] SEO Check:**
    - Does every page have a unique and descriptive `<title>` tag?
    - Does every page have a unique and compelling `<meta name="description">` tag?

- **[ ] Consistency Check:**
    - Does the navigation bar appear correctly on all pages?
    - Does the footer appear correctly on all pages?
    - Is the color scheme and font usage consistent with the established style?

- **[ ] Analytics Check:**
    - Does the page include the Google Analytics tracking code in the `<head>` section?

## How to Use This File
I will read this file at the beginning of each session to remind myself of the rules. I will verbally confirm that I have completed the pre-commit checklist before pushing any changes.
