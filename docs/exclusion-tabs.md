# Exclusion Tabs

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/exclusion-tabs)
> **Source Code**: [/src/animations/exclusion-tabs](/src/animations/exclusion-tabs)

## Tags
- `reanimated`
- `skia`

## What's This About?

Exclusion Tabs - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

## Usage

```tsx
type ExclusionTabsProps = {  tabs: string[];  activeTabIndex: number;  onTabChange: (tab: string) => void;  containerWidth: number;  height: number;};
// Basic usageconst tabs = ['Home', 'Changelog', 'Career', 'About'];
<ExclusionTabs  tabs={tabs}  activeTabIndex={0}  onTabChange={(tab) => {    console.log('Selected tab:', tab);  }}  containerWidth={windowWidth}  height={45}/>;
// With state managementconst [activeTabIndex, setActiveTabIndex] = useState(0);
<ExclusionTabs  tabs={tabs}  activeTabIndex={activeTabIndex}  onTabChange={(tab) => {    setActiveTabIndex(tabs.indexOf(tab));  }}  containerWidth={windowWidth}  height={45}/>;
```

GitHubAsk for support

Exclusion Tabs - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
