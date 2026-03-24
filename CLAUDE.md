# Raditex — Claude Code Workspace

## Project Overview
Raditex is an IT consultancy targeting Estonian SMEs (small and medium enterprises) without in-house IT departments. The brand positions itself as a reliable, accessible technology partner for businesses that need IT support without the complexity.

## Communication
- **Always respond in Estonian** unless the user writes in another language
- Use professional but approachable tone — no unnecessary jargon
- When writing client-facing content (website copy, proposals, emails), use Estonian

## Project Goals
- Build and maintain the Raditex website (HTML/CSS, no heavy frameworks)
- Create client-facing documents: proposals, assessments, service descriptions
- Automate repetitive IT consulting tasks where possible

## Tech Stack
- **Frontend:** HTML5, CSS3, vanilla JavaScript (keep it simple and fast)
- **Hosting:** Home server (Umbrel OS) or static hosting
- **Documents:** Node.js scripts for generating .docx and .pdf files
- **No heavy frameworks** unless explicitly requested

## Code Style
- Clean, readable code with comments in English
- Mobile-first responsive design
- Semantic HTML (use proper heading hierarchy, aria labels)
- CSS variables for colors and typography — never hardcode hex values
- No inline styles

## File Structure
```
raditex-workspace/
├── CLAUDE.md                  ← you are here
├── .claude/
│   └── commands/              ← custom slash commands
│       ├── new-proposal.md
│       ├── site-review.md
│       └── translate.md
├── src/
│   ├── index.html
│   ├── css/
│   ├── js/
│   └── assets/
├── docs/
│   ├── proposals/
│   ├── assessments/
│   └── templates/
└── assets/
    └── images/
```

## Brand Guidelines
- **Primary color:** #1a1a2e (dark navy)
- **Accent color:** #0f3460 (deep blue)
- **Highlight:** #e94560 (red accent)
- **Font:** Inter or system-ui
- **Tone:** Professional, trustworthy, approachable
- **Target audience:** Estonian SME owners and managers, non-technical

## Key Services (for website copy and proposals)
1. IT support and helpdesk
2. Cybersecurity assessments (ISKE framework, ISO 27001 aligned)
3. Network setup and maintenance
4. Cloud migration and setup
5. IT strategy consulting

## Document Templates
When generating proposals or assessments, always:
- Use the client's company name and contact person
- Reference Estonian standards (ISKE, GDPR/isikuandmete kaitse)
- Include pricing in EUR
- Add Raditex OÜ footer with contact details

## What NOT to do
- Do not use jQuery or Bootstrap unless explicitly asked
- Do not change navigation structure without asking first
- Do not delete existing content — always ask before removing
- Do not commit sensitive data (API keys, passwords, client info)

## Common Tasks
- `/new-proposal` — generate a new client proposal document
- `/site-review` — review the website for issues and improvements
- `/translate` — translate content between Estonian, English, and German
