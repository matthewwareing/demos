# Smooth Dropdown

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/smooth-dropdown)
> **Source Code**: [/src/animations/smooth-dropdown](/src/animations/smooth-dropdown)

## Tags
- `reanimated`

## What's This About?

This component creates an elegant dropdown menu with smooth animations and icon support. Each option in the dropdown can have an associated icon and label, and the component includes a customizable header. The implementation features smooth expand/collapse animations and selection handling, making it suitable for navigation menus or option selectors.

## Technical Implementation

The component uses:

- Animated transitions
- Icon integration
- Option selection
- Custom header
- Event handling

## Usage

```tsx
// Options configurationconst options = [  { label: 'Charts', iconName: 'barschart' },  { label: 'Book', iconName: 'book' },  { label: 'Calendar', iconName: 'calendar' },  { label: 'Camera', iconName: 'camera' }];
// Basic usage<SmoothDropdown />
// Dropdown with custom options<Dropdown  options={options}  header={{    label: 'Header',    iconName: 'ellipsis1'  }}  onPick={(value) => {    console.log('Selected:', value);  }}/>
// Typestype Option = {  label: string;  iconName: string;};
type DropdownProps = {  options: Option[];  header: Option;  onPick: (value: string) => void;};
```

GitHubAsk for support

Smooth Dropdown - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
