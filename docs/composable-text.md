# Composable Text

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/composable-text)
> **Source Code**: [/src/animations/composable-text](/src/animations/composable-text)

## Tags
- `reanimated`
- `react-native`

## Features

- Smooth per-character animations using Reanimated's Layout Animations
- Automatic character transitions with unique key bindings
- Customizable text and container styles
- Optimized performance for text changes

## Usage

```tsx
import { ComposableText } from 'composable-text';import { StyleSheet, TouchableOpacity } from 'react-native';
const MyComponent = () => {  const [text, setText] = useState('Use Max');
  return (    <TouchableOpacity      onPress={() =>        setText((prevText) =>          prevText === 'Use Max' ? 'Using Max' : 'Use Max'        )      }    >      <ComposableText        text={text}        style={styles.text}        containerStyle={styles.container}      />    </TouchableOpacity>  );};
```

GitHubAsk for support

Composable Text - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
