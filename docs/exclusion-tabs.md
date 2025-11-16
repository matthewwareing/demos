# Exclusion Tabs

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/exclusion-tabs)
> **Source Code**: [/src/animations/exclusion-tabs](/src/animations/exclusion-tabs)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## What's This About?

- Uses blend mode effects
- Handles tab switching
- Adapts to screen width
- Manages active tab state

## Usage

```typescript
type ExclusionTabsProps = {  tabs: string[];  activeTabIndex: number;  onTabChange: (tab: string) => void;  containerWidth: number;  height: number;};
// Basic usageconst tabs = ['Home', 'Changelog', 'Career', 'About'];
<ExclusionTabs  tabs={tabs}  activeTabIndex={0}  onTabChange={(tab) => {    console.log('Selected tab:', tab);  }}  containerWidth={windowWidth}  height={45}/>;
// With state managementconst [activeTabIndex, setActiveTabIndex] = useState(0);
<ExclusionTabs  tabs={tabs}  activeTabIndex={activeTabIndex}  onTabChange={(tab) => {    setActiveTabIndex(tabs.indexOf(tab));  }}  containerWidth={windowWidth}  height={45}/>;
```

---

*Documentation extracted from reactiive.io/demos*
