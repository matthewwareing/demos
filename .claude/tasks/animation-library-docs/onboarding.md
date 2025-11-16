# Animation Library Documentation - Onboarding

## Task Overview

Add comprehensive explainer documentation from [reactiive.io/demos](https://reactiive.io/demos) to the animations in the [enzomanuelmangano/demos](https://github.com/enzomanuelmangano/demos) GitHub repository.

### Goal
The GitHub repository contains 106 React Native animation demos, but lacks the detailed explainers that are available on the reactiive.io website. This project aims to extract those explainers and add them to the repository in a centralized `/docs` folder as markdown files.

---

## Repository Analysis

### Tech Stack
- **Framework**: React Native with Expo
- **Animation Libraries**:
  - React Native Reanimated
  - React Native Gesture Handler
  - React Native Skia
- **Package Manager**: Bun
- **Language**: TypeScript

### Repository Structure
```
demos/
├── src/
│   ├── animations/          # 106 animation folders
│   │   ├── action-tray/
│   │   ├── add-to-cart/
│   │   ├── airbnb-flip-interaction/
│   │   └── ... (103 more)
│   ├── navigation/
│   └── packages/
├── app/
├── assets/
├── .github/
└── README.md
```

### Animation Registry
All animations are cataloged in `src/animations/registry.ts`, which contains:
- `AnimationRegistry`: Maps slug → component
- `AnimationMetadata`: Maps slug → metadata (name, route, icon, etc.)

**Total Animations**: 106 unique animation demos

---

## Website Analysis

### Structure
- **Main Page**: https://reactiive.io/demos
- **Individual Demos**: https://reactiive.io/demos/{slug}
  - Example: https://reactiive.io/demos/airbnb-flip-interaction

### Explainer Content Structure
Each demo page on reactiive.io contains:

1. **Header**
   - Title (e.g., "Airbnb Flip Interaction with Reanimated")
   - Publication date
   - Video/animation preview
   - QR code for mobile testing

2. **Tags**
   - Technology tags (e.g., `reanimated`, `expo-blur`, `gesture-handler`)

3. **Description**
   - Brief overview paragraph

4. **What it does**
   - Detailed explanation of the animation behavior
   - User interaction flow
   - Visual effects described

5. **Usage**
   - Code examples with syntax highlighting
   - Import statements
   - Component usage examples
   - TypeScript type definitions

6. **Additional Sections** (varies by demo)
   - Implementation details
   - Technical notes
   - Related demos

---

## Animation Mapping

A complete mapping of all 106 animations has been created in `animation_mapping.json`:

```json
{
  "slug": "airbnb-flip-interaction",
  "name": "Airbnb Flip Interaction",
  "websiteUrl": "https://reactiive.io/demos/airbnb-flip-interaction",
  "folderPath": "src/animations/airbnb-flip-interaction",
  "docsPath": "docs/airbnb-flip-interaction.md"
}
```

### Key Findings
- ✅ All 106 animations in the repository appear to have corresponding pages on reactiive.io
- ✅ Slug naming is consistent between repository folders and website URLs
- ✅ No obvious gaps or mismatches found

---

## Complete Animation List

<details>
<summary>All 106 Animations (click to expand)</summary>

1. action-tray - Action Tray
2. add-to-cart - Add to Cart
3. airbnb-flip-interaction - Airbnb Flip Interaction
4. airbnb-slider - AirBnb Slider
5. alert-drawer - Alert Drawer
6. animated-3d-parallax - Animated 3D Parallax
7. animated-clip-box - Animated Clip Box
8. animated-count-text - Animated Count Text
9. animated-grid-list - Animated Grid List
10. animated-indicator-list - Animated Indicator List
11. atlas-button - Atlas Button
12. atlas-sphere - Atlas Sphere
13. audio-player - AudioPlayer
14. balance-slider - Balance Slider
15. bezier-curve-outline - Bezier Curve Outline
16. blur-cards - Blur Cards
17. blur-circles - Blur Circles
18. blurred-bottom-bar - Blurred Bottom Bar
19. blurred-scroll - Blurred Scroll
20. bottom-bar-skia - BottomBarSkia
21. card-shader-reflections - Card Shader Reflections
22. checkbox-interactions - Checkbox Interactions
23. circular-carousel - Circular Carousel
24. clerk-toast - Clerk Toast
25. clock-time-picker - Clock Time Picker
26. color-carousel - Color Carousel
27. composable-text - Composable Text
28. coverflow-carousel - Coverflow Carousel
29. cuberto-slider - Cuberto Slider
30. delete-button - Delete Button
31. dot-sheet - Dot Sheet
32. drag-to-sort - Drag to Sort
33. draggable-panel - Draggable Panel
34. duration-slider - Duration Slider
35. dynamic-blur-tabs - Dynamic Blur Tabs
36. dynamic-tab-indicator - Dynamic Tab Indicator
37. email-demo - Email Demo
38. empty-qr-code - Empty QR Code
39. everybody-can-cook - Everybody Can Cook
40. exclusion-tabs - Exclusion Tabs
41. expandable-mini-player - Expandable Mini Player
42. family-number-input - Family Number Input
43. fibonacci-shader - Fibonacci Shader
44. fibonacci-shader-grid - Fibonacci Shader Grid
45. floating-bottom-bar - Floating Bottom Bar
46. floating-modal - Floating Modal
47. fluid-slider - Fluid Slider
48. fluid-tab-interaction - Fluid Tab Interaction
49. fourier-visualizer - Fourier Visualizer
50. fractal-glass - Fractal Glass
51. geometry-button - Geometry Button
52. github-contributions - GitHub Contributions
53. github-onboarding - GitHub Onboarding
54. gl-transitions - GL Transitions
55. grid-visualizer - Grid Visualizer
56. image-cropper - Image Cropper
57. imessage-stack - iMessageStack
58. infinite-carousel - Infinite Carousel
59. interaction-appearance - Interaction Appearance
60. ios-home-bouncy - iOS Home Bouncy
61. ios-home-grid - iOS Home Grid
62. linear-sensors - Linear Sensors
63. liquid-glass-playground - Liquid Glass Playground
64. loading-button - Loading Button
65. magnet-spring - Magnet Spring
66. metaball - Metaball
67. miles-bar-chart - Miles Bar Chart
68. mnist - MNIST
69. mobile-input - Mobile Input
70. motion-blur - Motion Blur
71. online-offline - Online Offline
72. paper-folding - Paper Folding
73. particles-button - Particles Button
74. pomodoro-timer - Pomodoro Timer
75. popup-handler - Popup Handler
76. prequel-slider - Prequel Slider
77. qr-code-generator - QR Code Generator
78. radar-chart - Radar Chart
79. record-button - Record Button
80. scroll-progress - Scroll Progress
81. scroll-transition-3d - 3D Scroll Transition
82. scrollable-bottom-sheet - Scrollable Bottom Sheet
83. selectable-grid-list - Selectable Grid List
84. shake-to-delete - Shake to Delete
85. shared-transitions - Shared Transitions
86. skia-bottom-sheet - Skia BottomSheet
87. skia-color-picker - Skia Color Picker
88. slide-to-reveal - Slide to Reveal
89. smooth-dropdown - Smooth Dropdown
90. snake - Snake
91. spiral - Spiral
92. split-button - Split Button
93. stacked-bottom-sheet - Stacked Bottom Sheet
94. stacked-carousel - Stacked Carousel
95. stacked-list - Stacked List
96. stacked-modals - Stacked Modals
97. staggered-card-number - Staggered Card Number
98. steddy-graph-interaction - Steddy Graph Interaction
99. steps - Steps
100. story-list - Story List
101. sudoku - Sudoku
102. tab-navigation - Tab Navigation
103. telegram-theme-switch - Telegram Theme Switch
104. theme-canvas-animation - Theme Canvas Animation
105. threads-holo-ticket - Threads Holo Ticket
106. time-machine - Time Machine
107. toast - Toast
108. twitter-tab-bar - Twitter Tab Bar
109. twodos-slide - Twodos Slide
110. verification-code - Verification Code
111. verification-code-face - Verification Code Face
112. wheel-picker - Wheel Picker

</details>

---

## Implementation Plan

### Planned Documentation Structure

```
demos/
├── docs/
│   ├── README.md                      # Index of all animations with links
│   ├── action-tray.md                 # Individual explainers
│   ├── add-to-cart.md
│   ├── airbnb-flip-interaction.md
│   └── ... (106 markdown files total)
├── src/
│   └── animations/
│       └── ... (existing structure)
└── README.md                          # Updated to link to /docs
```

### Markdown Template

Each animation's markdown file should follow this structure:

```markdown
# {Animation Name}

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/{slug})
> **Source Code**: [/src/animations/{slug}](/src/animations/{slug})

## Tags
- {tag1}
- {tag2}

## Description
{Brief description paragraph}

## What it does
{Detailed explanation}

## Usage
{Code examples}

## Additional Notes
{Any other relevant information}

---
*Documentation extracted from reactiive.io/demos*
```

---

## Content Extraction Challenges

### Challenge: JavaScript-Rendered Content
The reactiive.io website is built with React/Expo Web, meaning:
- Content is rendered client-side with JavaScript
- Simple HTTP requests return minimal HTML
- The actual content is loaded dynamically

### Attempted Solutions

1. ✅ **Simple HTTP scraping** - Basic curl/fetch requests
   - Result: Only gets empty HTML shell

2. ✅ **BeautifulSoup parsing** - Python HTML parser
   - Result: Cannot parse JavaScript-rendered content

3. ❌ **Required: Browser automation** - Playwright, Puppeteer, or Selenium
   - Would allow JavaScript execution
   - Can extract fully-rendered content
   - More complex setup required

---

## Recommended Approaches

### Option 1: Automated Scraping (Recommended for scale)

Use Playwright or Puppeteer to:
1. Navigate to each demo URL
2. Wait for content to load
3. Extract HTML from rendered page
4. Parse and convert to markdown
5. Save to respective docs file

**Tools needed**:
- Playwright or Puppeteer
- HTML-to-Markdown converter
- Node.js script to orchestrate

**Pros**:
- Automated for all 106 animations
- Consistent formatting
- Reproducible process

**Cons**:
- More complex setup
- Requires browser automation

### Option 2: Manual Extraction (Recommended for quick start)

For a quick proof of concept:
1. Manually visit 3-5 popular animations
2. Copy the explainer content
3. Format as markdown
4. Use as templates for automated extraction

**Popular animations to start with**:
- airbnb-flip-interaction
- floating-bottom-bar
- swipe-cards
- shared-transitions
- circular-carousel

### Option 3: Hybrid Approach (Recommended overall)

1. Create the docs folder structure
2. Generate placeholder markdown files for all 106 animations
3. Manually populate 5-10 key animations
4. Use automated tool to fill in the rest

---

## Repository State

### What's Been Done ✅

1. **Forked Repository**
   - Fork URL: https://github.com/matthewwareing/demos
   - Cloned locally to: `/Users/matthewwareing/apps/demos`

2. **Repository Analysis**
   - Identified 106 animations in `src/animations/`
   - Analyzed `registry.ts` for complete animation list
   - Documented tech stack and structure

3. **Mapping Created**
   - Generated `animation_mapping.json` with all 106 animations
   - Includes: slug, name, website URL, folder path, and planned docs path

4. **Content Analysis**
   - Examined demo page structure on reactiive.io
   - Documented explainer format and sections
   - Identified JavaScript-rendering challenge

### What's Next ⏭️

1. **Create /docs folder structure**
   - Create `/docs` directory in the repository
   - Generate placeholder markdown files for each animation

2. **Extract explainer content**
   - Set up Playwright/Puppeteer for scraping
   - OR manually extract content for initial animations
   - Convert HTML content to markdown

3. **Generate documentation files**
   - Populate markdown files with extracted content
   - Follow consistent template
   - Include proper links and formatting

4. **Create docs/README.md**
   - Index page with links to all animations
   - Organized by category/alphabetically
   - Include description and quick navigation

5. **Update main README.md**
   - Add link to `/docs` folder
   - Mention documentation availability
   - Explain how to browse animations

6. **Commit and push**
   - Commit all changes with clear message
   - Push to forked repository
   - Optionally create PR to upstream

---

## Key Files Reference

### In Forked Repository
- **Animation source**: `/demos/src/animations/{slug}/`
- **Registry**: `/demos/src/animations/registry.ts`
- **Package info**: `/demos/package.json`
- **Main README**: `/demos/README.md`

### In Working Directory
- **Mapping**: `/Users/matthewwareing/apps/animation_mapping.json`
- **Scraper script**: `/Users/matthewwareing/apps/scrape_demos.py`
- **Mapping script**: `/Users/matthewwareing/apps/create_animation_mapping.js`

---

## Useful Commands

### Repository Navigation
```bash
cd /Users/matthewwareing/apps/demos
```

### Install Dependencies
```bash
cd demos
bun install
```

### Run iOS App
```bash
bun ios
```

### Run Android App
```bash
bun android
```

### List All Animations
```bash
ls -la demos/src/animations/
```

---

## Additional Resources

- **Main Repository**: https://github.com/enzomanuelmangano/demos
- **Forked Repository**: https://github.com/matthewwareing/demos
- **Website**: https://reactiive.io/demos
- **Animation Mapping**: `/Users/matthewwareing/apps/animation_mapping.json`
- **Author**: Enzo Manuel Mangano (@reactiive_)
- **Course**: https://reanimate.dev

---

## Notes

- The repository uses a custom license that allows free use but prohibits redistribution
- All animations are built with React Native Reanimated 3.x
- The website and repository are actively maintained
- Some animations have special flags (e.g., `alert: true` for experimental features)
- The project includes TestFlight distribution for iOS

---

**Last Updated**: 2025-11-16
**Status**: Repository analyzed, mapping created, ready for content extraction
