# Alert Drawer

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/alert-drawer)
> **Source Code**: [/src/animations/alert-drawer](/src/animations/alert-drawer)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Usage

```typescript
type AlertDrawerProps = {  title: string;  description: string;  buttonLabel: string;  onConfirm?: () => void;};
// Example usage<AlertDrawer  title="Are you sure?"  description="Confirmation message here"  buttonLabel="Continue"  onConfirm={() => console.log('Confirmed')}/>;
```

---

*Documentation extracted from reactiive.io/demos*
