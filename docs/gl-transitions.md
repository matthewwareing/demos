# GL Transitions

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/gl-transitions)
> **Source Code**: [/src/animations/gl-transitions](/src/animations/gl-transitions)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

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

---

*Documentation extracted from reactiive.io/demos*
