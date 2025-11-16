# Scroll Progress

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/scroll-progress)
> **Source Code**: [/src/animations/scroll-progress](/src/animations/scroll-progress)

## Tags
- `reanimated`

## What's This About?

This component creates a sophisticated scrollable content interface with a progress indicator. It tracks reading progress through sections of content, calculates estimated reading time, and provides smooth scroll animations. The implementation includes precise scroll position tracking, progress calculations, and a reset functionality, making it perfect for long-form content or article readers.

## Technical Implementation

The component uses:

- Scroll position tracking
- Reading time calculation
- Progress indicators
- Reset functionality
- Layout measurements

## Usage

```tsx
// Data structuretype Section = {  title: string;  description: string;};
// Basic usage<ScrollProgress />
// Section list with custom rendering<SectionContentList  sections={sections}  renderSection={(section, index) => (    <View key={index}>      <Text>{section.title}</Text>      <Text>{section.description}</Text>    </View>  )}  contentContainerStyle={{    paddingHorizontal: 20,    paddingTop: 20,    paddingBottom: 100  }}/>
// Progress calculationconst scrollableHeight = useDerivedValue(() => {  return scrollHeight.value - viewHeight.value + paddingBottom;});
const progress = clamp(  scrollOffset / scrollableHeight,  0,  1);
```

GitHubAsk for support

Scroll Progress - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
