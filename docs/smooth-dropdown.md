# Smooth Dropdown

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/smooth-dropdown)
> **Source Code**: [/src/animations/smooth-dropdown](/src/animations/smooth-dropdown)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Animated transitions
- Icon integration
- Option selection
- Custom header
- Event handling

## Usage

```typescript
// Options configurationconst options = [  { label: 'Charts', iconName: 'barschart' },  { label: 'Book', iconName: 'book' },  { label: 'Calendar', iconName: 'calendar' },  { label: 'Camera', iconName: 'camera' }];
// Basic usage<SmoothDropdown />
// Dropdown with custom options<Dropdown  options={options}  header={{    label: 'Header',    iconName: 'ellipsis1'  }}  onPick={(value) => {    console.log('Selected:', value);  }}/>
// Typestype Option = {  label: string;  iconName: string;};
type DropdownProps = {  options: Option[];  header: Option;  onPick: (value: string) => void;};
```

---

*Documentation extracted from reactiive.io/demos*
