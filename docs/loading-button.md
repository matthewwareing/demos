# Loading Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/loading-button)
> **Source Code**: [/src/animations/loading-button](/src/animations/loading-button)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- State transitions
- Gesture handling
- Async operations
- Visual feedback

## Usage

```typescript
// Basic usage with state managementconst { status, mutateAsync } = useMutation(async () => {  // Your async operation  await someAsyncOperation();});
<LoadingButton  status={status}  onPress={async () => {    await mutateAsync();  }}  style={{    height: 60,    borderRadius: 25,  }}  colorFromStatusMap={{    idle: '#47A1E6',    loading: '#47A1E6',    success: '#5BC682',    error: '#CD5454',  }}  titleFromStatusMap={{    idle: 'Check Transaction',    loading: 'Analyzing Transaction',    success: 'Transaction Safe',    error: 'Transaction Unsafe',  }}/>;
```

---

*Documentation extracted from reactiive.io/demos*
