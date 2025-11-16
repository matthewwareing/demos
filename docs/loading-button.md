# Loading Button

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/loading-button)
> **Source Code**: [/src/animations/loading-button](/src/animations/loading-button)

## Tags
- `reanimated`
- `skia`

## What's This About?

This component creates an interactive button that provides visual feedback for asynchronous operations. The button smoothly transitions between different states (idle, loading, success, error) with appropriate colors and text labels. It integrates with React Query for handling asynchronous state management and includes configurable timeouts and retry logic for robust error handling.

## Technical Implementation

The component uses:

- State transitions
- Gesture handling
- Async operations
- Visual feedback

## Usage

```tsx
// Basic usage with state managementconst { status, mutateAsync } = useMutation(async () => {  // Your async operation  await someAsyncOperation();});
<LoadingButton  status={status}  onPress={async () => {    await mutateAsync();  }}  style={{    height: 60,    borderRadius: 25,  }}  colorFromStatusMap={{    idle: '#47A1E6',    loading: '#47A1E6',    success: '#5BC682',    error: '#CD5454',  }}  titleFromStatusMap={{    idle: 'Check Transaction',    loading: 'Analyzing Transaction',    success: 'Transaction Safe',    error: 'Transaction Unsafe',  }}/>;
```

GitHubAsk for support

Loading Button - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
