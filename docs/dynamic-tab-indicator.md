# Dynamic Tab Indicator

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/dynamic-tab-indicator)
> **Source Code**: [/src/animations/dynamic-tab-indicator](/src/animations/dynamic-tab-indicator)

## Tags
- `reanimated`

## Description

Scan to try on your device

## What's This About?

- Adjusts indicator width to tab content
- Animates between tab selections
- Supports custom data input
- Handles dynamic content sizes

## Technical Implementation

- Reanimated for smooth transitions
- Dynamic width calculations
- Tab content measurements
- Custom data mapping

## Usage

```typescript
type TabData = {  id: string;  title: string;  // other data properties};
// Basic usageconst data: TabData[] = [  { id: '1', title: 'Tab 1' },  { id: '2', title: 'Tab 2' },  // ...more tabs];
<DynamicTabIndicator data={data} />;
```

---

*Documentation extracted from reactiive.io/demos*
