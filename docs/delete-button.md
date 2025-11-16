# Delete Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/delete-button)
> **Source Code**: [/src/animations/delete-button](/src/animations/delete-button)

## Tags
- `skia`

## Description

Scan to try on your device

## What's This About?

- Smooth expansion animation with a gooey effect
- Close button that appears during confirmation
- Dynamic text transitions between states
- Gesture-based interactions
- Customizable dimensions and text

## Technical Implementation

- Gooey effect using Skia layer blending
- Complex gesture handling with Skia touch events
- Multiple coordinated animations:Button expansion/contractionColor transitionsText opacity and positionClose button reveal
- Button expansion/contraction
- Color transitions
- Text opacity and position
- Close button reveal
- Custom font handling

## Usage

```typescript
type DeleteButtonProps = {  onConfirmDeletion: () => void;  height: number;  width: number;  initialText?: string;  confirmText?: string;  additionalWidth: number;  closeOnConfirm?: boolean;};
// Basic usage<DeleteButton  height={50}  width={150}  additionalWidth={80}  onConfirmDeletion={() => {    console.log('Confirmed deletion');  }}/>
// Customized version<DeleteButton  height={50}  width={150}  additionalWidth={80}  initialText="Remove"  confirmText="Sure?"  closeOnConfirm={true}  onConfirmDeletion={() => {    handleDeletion();  }}/>
```

---

*Documentation extracted from reactiive.io/demos*
