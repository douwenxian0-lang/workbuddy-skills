---
name: motionsites-prompt
description: >
  Generate structured prompts for AI web design tools (Bolt, Lovable, Claude Code, Cursor) 
  following the MotionSites format. Use when user wants to create Hero sections, landing pages, 
  or web designs with React, Tailwind CSS, and Framer Motion. Trigger keywords: 
  "create hero section", "generate landing page", "motionsites prompt", "web design prompt"
agent_created: true
---

# MotionSites Prompt Generator

Generate professional web design prompts using the MotionSites structured format.

## Usage

When user requests web design/hero section creation, generate a prompt following this format:

## Prompt Structure

```
I. Metadata
- Project: [project name]
- Style: [modern/minimalist/brutalist/editorial]
- Tech Stack: React + Tailwind CSS + Framer Motion
- Requirements: [key requirements]

II. Video Preview (Optional)
[Describe any video/animation preview if applicable]

III. Implementation Prompt
Create a [description] using:
- React + TypeScript
- Tailwind CSS for styling
- Framer Motion for animations
- Responsive design (mobile-first)
- [Specific components/features]

IV. Export & Integration
- Output format: [component/files]
- Integration: [how to integrate]
```

## Example

**User Request**: "Create a modern SaaS hero section"

**Generated Prompt**:
```
I. Metadata
- Project: SaaS Landing Page Hero
- Style: Modern, clean, professional
- Tech Stack: React + Tailwind CSS + Framer Motion
- Requirements: Email capture, animated headline, CTA buttons

II. Implementation Prompt
Create a hero section component with:
- Animated headline with word rotation
- Email input with validation
- Two CTA buttons (primary/secondary)
- Background gradient with subtle pattern
- Responsive: stacked on mobile, side-by-side on desktop
- Framer Motion animations: fade-in, slide-up

III. Export
- Single React component: HeroSection.tsx
- Tailwind config with custom colors
- Framer Motion variants object
```

## Notes

- Always specify "React + Tailwind CSS + Framer Motion" as tech stack
- Include specific animation requirements
- Mention responsive design
- Ask for component-based architecture
