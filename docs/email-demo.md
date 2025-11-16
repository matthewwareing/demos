# Email Demo

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/email-demo)
> **Source Code**: [/src/animations/email-demo](/src/animations/email-demo)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

Email Demo - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

## Technical Implementation

The component uses:

- Reanimated for list animations
- Shared values for state management
- Custom hooks for shake animations
- Linear gradients for visual effects
- List virtualization for performance

## Usage

```tsx
type EmailItem = {  id: string;  title: string;  content: string;};
// Basic usage<EmailDemo />;
// List item configurationconst ITEM_HEIGHT = 100;const ITEM_MARGIN = 10;
// Custom list implementation<InteractiveList  data={items}  itemHeight={ITEM_HEIGHT + ITEM_MARGIN}  amountToShift={erasedItems}  renderItem={({ item }) => <ListItem item={item} itemHeight={ITEM_HEIGHT} />}/>;
```

GitHubAsk for support

Email Demo - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
