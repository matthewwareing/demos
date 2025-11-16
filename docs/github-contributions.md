# GitHub Contributions

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/github-contributions)
> **Source Code**: [/src/animations/github-contributions](/src/animations/github-contributions)

## Tags
- `reanimated`

## The Code Structure

```typescript
src/├── contribution-calendar/│   ├── index.tsx                    # Main calendar component│   ├── contribution-square.tsx      # Individual animated squares│   ├── types.tsx                    # TypeScript definitions│   └── utils/│       ├── animation-utils.tsx      # Animation timing calculations│       └── date-utils.tsx           # Date handling utilities├── config/│   └── defaults.tsx                 # Color schemes and settings├── contribution-data.tsx            # Sample data generator└── index.tsx                        # App entry point
```

## Features

- Smooth Animations: Spring-based animations with configurable timing
- Multiple Color Schemes: GitHub green, blue, and purple themes
- Responsive Design: Adapts to different screen sizes automatically
- TypeScript Support: Fully typed for better development experience
- Touch Interaction: Tap anywhere to start/stop animations
- Realistic Data: Generates sample contribution data or accepts custom data

### Custom Data Format

Provide your own contribution data using the ContributionData format:

```tsx
import { ContributionData } from './src/contribution-calendar/types';
const customData: ContributionData = {  '2024-01-01': 3, // High activity  '2024-01-02': 1, // Low activity  '2024-01-03': 0, // No activity  '2024-01-04': 4, // Very high activity  '2024-01-05': 2, // Medium activity  // ... more dates};
<GitHubContributionCalendar data={customData} />;
```

### Color Schemes

Choose from predefined color schemes or create your own:

```tsx
import { COLOR_SCHEMES } from './src/config/defaults';
// Predefined schemes<GitHubContributionCalendar colorScheme={COLOR_SCHEMES.github} /><GitHubContributionCalendar colorScheme={COLOR_SCHEMES.blue} /><GitHubContributionCalendar colorScheme={COLOR_SCHEMES.purple} />
// Custom schemeconst customScheme = {  level0: '#f1f8ff',  // No contributions  level1: '#c6e48b',  // Low  level2: '#7bc96f',  // Medium  level3: '#239a3b',  // High  level4: '#196127',  // Very high};
<GitHubContributionCalendar colorScheme={customScheme} />
```

GitHubAsk for support

Github Contributions - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
