---
name: awesome-readme-style
description: Guidelines and style preferences for updating my GitHub Profile README and other project READMEs. Ensures they match my specific personality, tone, formatting quirks, and gaming/anime references.
---

# README Style Guidelines

When generating or updating my GitHub profile README or other personal documentation, strictly follow these stylistic guidelines, structural patterns, and personality traits to ensure it sounds like *me*.

## 1. Tone and Personality
- **Conversational and Human**: Write as if a real person is speaking. Avoid overly formal corporate speak. Use natural phrasing, short punchy sentences, and blockquotes for emphasis.
- **Geeky but Not Forced**: Incorporate organic references to gaming, anime, and nerd culture.
  - *Approved References*: World of Warcraft (raiding/mains), Civilization (tech trees), Hunter x Hunter (Nen mastery analogy), SimCity (urban planning for code architecture), One Piece (Grand Line, pirate themes), Evangelion, Tabletop RPGs, Counter-Strike.
  - Do not force these references; weave them into legitimate points about software architecture and hobbies.
- **Engineering Philosophy**: Emphasize clean separation of concerns, OpenAPI contracts, TypeScript, and writing code for humans over compilers. Show a bias for fast feedback loops and CI/CD. Emphasize that "Good architecture is invisible."
- **AI Stance**: Present AI as a force multiplier. Emphasize that "AI generates, but *I* design." Highlight a philosophy of continuous learning and adopting whatever tool brings value today, not last decade.

## 2. Formatting Preferences
- **No Boring YAML or Bullet Lists**: Do not use generic YAML blocks or standard markdown tables for things that can be presented in a more "developer-native" way.
- **Developer-Native Code Zones**:
  - Use `git log --oneline` mockups to show career progression or timelines.
  - Use `diff` blocks to contrast bad practices (red) with good engineering standards (green).
  - Use `json` blocks for "Character Loadouts", personal stats, or hobbies.
  - Use terminal `bash` tree output (`tree -a`) to list side projects instead of standard Markdown tables.
  - Use `typescript` interfaces to boldly define engineering standards or rules.
- **Emojis & Icons**:
  - Liberally use standard emojis to add color (`🚀`, `🧠`, `🤖`, `🎮`, `🏗️`).
  - **Important Flag Rule**: Do not use standard flag emojis (e.g., 🇫🇷) directly in text, as they render as two-letter text codes (like "FR") on Windows. Instead, use an inline `<img>` tag with the official Twemoji SVG set to 14x14px so it perfectly matches the text height. Example: 
    `<img src="https://raw.githubusercontent.com/jdecked/twemoji/master/assets/svg/1f1eb-1f1f7.svg" width="14" height="14" alt="FR" />`

## 3. Visual Layout Elements
- **Tech Stack**: Combine related tools under broader category headings to reduce vertical whitespace (e.g., "Backend, Data & Testing"). Use `flat-square` shields.io badges (`style=flat-square`).
- **Retro HTML Features**: Use HTML `<marquee behavior="scroll" direction="left" scrollamount="6">` for footer or Call-To-Action text to give a nostalgic Web 1.0 feel. Use inline `<b>` tags inside the marquee (Markdown `**bold**` breaks inside marquees).
- **Custom Mascot/Portfolio Link**: Instead of generic `shields.io` badges for my portfolio, use a custom theme-appropriate image (like a 16-bit pirate rabbit `mascot-rabbit.png`) inside an `<a>` tag, paired with a bold text call-to-action to visit the site.
- **Dividers**: Use a `<div align="center">` paired with `###` headings, sandwiched by `---` standard markdown horizontal rules and `<!-- HTML comment blocks -->` to create clear, centered section headers.

## 4. What to Avoid
- **No Personal PII**: Do not list exact phone numbers, specific addresses, or highly sensitive info.
- **No Wall of Text**: Keep paragraphs short and punchy.
- **No Generic Intros**: Avoid corporate intros like "I am a passionate developer with X years of experience." Make it read like a story.
