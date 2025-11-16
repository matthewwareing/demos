# Tab Navigation

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/tab-navigation)
> **Source Code**: [/src/animations/tab-navigation](/src/animations/tab-navigation)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Tab management
- State handling
- Smooth transitions
- Active tracking
- Custom styling

## Usage

```typescript
// Basic usage<TabNavigation />
// Tabs component<Tabs  tabs={TABS_DATA}  activeTabIndex={activeTabIndex}  setActiveTabIndex={setActiveTabIndex}/>
// Tab state managementconst [activeTabIndex, setActiveTabIndex] = useState(0);
// Tab data structureconst TABS_DATA = [  {    id: 'tab1',    title: 'Tab 1',    content: 'Content 1'  },  {    id: 'tab2',    title: 'Tab 2',    content: 'Content 2'  }];
// Stylingconst styles = StyleSheet.create({  container: {    flex: 1,    backgroundColor: '#fff',    alignItems: 'center',    justifyContent: 'center'  }});
```

---

*Documentation extracted from reactiive.io/demos*
