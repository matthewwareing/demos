# GL Transitions

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/gl-transitions)
> **Source Code**: [/src/animations/gl-transitions](/src/animations/gl-transitions)

## Tags
- `reanimated`
- `skia`

## What's This About?

This component enhances navigation transitions using WebGL shaders. It provides a collection of pre-built transitions like DirectionalWarp, LinearBlur, CrossZoom, and Hexagonalize, which can be easily swapped to create different visual effects during screen navigation. The transitions are powered by GLSL shaders and can be extended with custom transitions from the GL Transitions gallery.

## Technical Implementation

The component uses:

- WebGL shaders
- Navigation integration
- GLSL transitions
- Screen management
- Custom providers

## Usage

```tsx
// Available transitionsimport {  DirectionalWarp,  LinearBlur,  CrossZoom,  Hexagonalize,} from './the-magic';
// Basic usage with a transition<GLTransitionsProvider transition={DirectionalWarp}>  <NavigationContainer>    <Stack.Navigator>      <Stack.Screen name="Home" component={HomeScreen} />      <Stack.Screen name="AddNote" component={AddNoteScreen} />    </Stack.Navigator>  </NavigationContainer></GLTransitionsProvider>;
// Custom transitions can be added from:// https://gl-transitions.com/gallery
```

GitHubAsk for support

Gl Transitions - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
