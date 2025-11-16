# Email Demo

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/email-demo)
> **Source Code**: [/src/animations/email-demo](/src/animations/email-demo)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## What's This About?

- Delete and restore actions
- Shake feedback for invalid actions
- Gradient overlays for depth
- Safe area handling

## Technical Implementation

- Reanimated for list animations
- Shared values for state management
- Custom hooks for shake animations
- Linear gradients for visual effects
- List virtualization for performance

## Usage

```typescript
type EmailItem = {  id: string;  title: string;  content: string;};
// Basic usage<EmailDemo />;
// List item configurationconst ITEM_HEIGHT = 100;const ITEM_MARGIN = 10;
// Custom list implementation<InteractiveList  data={items}  itemHeight={ITEM_HEIGHT + ITEM_MARGIN}  amountToShift={erasedItems}  renderItem={({ item }) => <ListItem item={item} itemHeight={ITEM_HEIGHT} />}/>;
```

---

*Documentation extracted from reactiive.io/demos*
