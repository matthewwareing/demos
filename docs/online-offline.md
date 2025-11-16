# Online Offline

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/online-offline)
> **Source Code**: [/src/animations/online-offline](/src/animations/online-offline)

## Tags
- `reanimated`
- `skia`
- `react-native`

## What it does

The component shows two groups of user avatars side by side. Online users appear on the left with full color photos, while offline users are shown on the right in grayscale. Each group has a subtle background pill that resizes as users move between states.

When a user's status changes, their avatar slides from one group to the other with a spring animation. The component handles all the layout calculations and animations automatically.

## Demo

Tap anywhere on the screen to see a random user change their status. The selected avatar will move to its new group and the grayscale filter will fade in or out accordingly.

## Technical details

Built with React Native, React Native Reanimated for animations, and React Native Skia for the grayscale color filter.

You should probably avoid using Skia for rendering images in this specific case, as it requires multiple canvases.

A more practical approach would be to use expo-image with a native grayscale filter (for example, react-native-color-matrix-image-filters). However, you won't get the smooth color interpolation effect while transitioning between online and offline states (which is something I really cared about in this demo 😅).

Since I wanted animations that are quick to test in development mode, I opted for Skia as it works perfectly with Expo Go. In a production app, I would probably use the expo-image approach.

GitHubAsk for support

Online Offline - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
