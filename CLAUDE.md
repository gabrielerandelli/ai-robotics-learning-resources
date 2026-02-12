# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a documentation-only repository containing a curated collection of learning resources for AI, Robotics, Agents, and Vibe Coding. There is no source code, build system, or tests.

## Structure

The entire content is in README.md, organized into four main sections:
- **AI (Generic Track)** - Courses, projects, whitepapers, research papers, blogs, books, videos
- **Vibe Coding** - Courses, projects & tools, blogs, videos
- **Agents** - Courses, projects & protocols (ADK, MCP, A2A)
- **Robotics** - Courses

## Contribution Guidelines

When adding new resources:
- Use markdown table format matching existing sections
- Include resource name as a link and a brief description
- For research papers, include authors and date
- For videos, include date
- Place entries in appropriate category sections
- Place entries in descending order by publish date, whenever available in the section

## GitHub Guidelines
- never commit links.txt file

## Link validity
- Before commiting, navigate all the existing links to double check if they're still available. If not anymore, remove them. Use three agents in parallel for doing this.
- Before commiting, navigate all new existing links to double check if they're reachable. If not, let me know

## Duplication check
- Check for duplicates before considering a new link to add to README.md

## Self-improvement
- update @CLAUDE.md in this folder before committing, if during the current conversation you have learned something that could ease the process next time

## Playwright Setup (if needed)
If Playwright browser is not installed, run:
```bash
npx playwright install chromium
```

If system libraries are missing (e.g., `libxkbcommon.so.0`), install them:
```bash
sudo apt-get install -y libxkbcommon0 libglib2.0-0 libnss3 libnspr4 libdbus-1-3 libatk1.0-0 libatk-bridge2.0-0 libcups2 libdrm2 libxcomposite1 libxdamage1 libxfixes3 libxrandr2 libgbm1 libpango-1.0-0 libcairo2 libasound2t64 libatspi2.0-0
```

To take screenshots for link verification:
```bash
npx playwright screenshot --wait-for-timeout 5000 "<URL>" /tmp/screenshot.png
```

Note: WebFetch does not work with X/Twitter or YouTube - use Playwright instead for these sites.
