# Scroll Progress

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/scroll-progress)
> **Source Code**: [/src/animations/scroll-progress](/src/animations/scroll-progress)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Scroll position tracking
- Reading time calculation
- Progress indicators
- Reset functionality
- Layout measurements

## Usage

```typescript
// Data structuretype Section = {  title: string;  description: string;};
// Basic usage<ScrollProgress />
// Section list with custom rendering<SectionContentList  sections={sections}  renderSection={(section, index) => (    <View key={index}>      <Text>{section.title}</Text>      <Text>{section.description}</Text>    </View>  )}  contentContainerStyle={{    paddingHorizontal: 20,    paddingTop: 20,    paddingBottom: 100  }}/>
// Progress calculationconst scrollableHeight = useDerivedValue(() => {  return scrollHeight.value - viewHeight.value + paddingBottom;});
const progress = clamp(  scrollOffset / scrollableHeight,  0,  1);
```

---

*Documentation extracted from reactiive.io/demos*
