# Delete Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/delete-button)
> **Source Code**: [/src/animations/delete-button](/src/animations/delete-button)

## Tags
- `skia`

## What's This About?

This component creates an interactive delete button that expands to reveal a confirmation state. It features:

## Technical Implementation

The component leverages Skia for high-performance rendering and implements:

- Gooey effect using Skia layer blending
- Complex gesture handling with Skia touch events
- Multiple coordinated animations:Button expansion/contractionColor transitionsText opacity and positionClose button reveal
- Button expansion/contraction
- Color transitions
- Text opacity and position
- Close button reveal
- Custom font handling

## Usage

```tsx
type DeleteButtonProps = {  onConfirmDeletion: () => void;  height: number;  width: number;  initialText?: string;  confirmText?: string;  additionalWidth: number;  closeOnConfirm?: boolean;};
// Basic usage<DeleteButton  height={50}  width={150}  additionalWidth={80}  onConfirmDeletion={() => {    console.log('Confirmed deletion');  }}/>
// Customized version<DeleteButton  height={50}  width={150}  additionalWidth={80}  initialText="Remove"  confirmText="Sure?"  closeOnConfirm={true}  onConfirmDeletion={() => {    handleDeletion();  }}/>
```

GitHubAsk for support

Delete Button - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
