# Card Shader Reflections

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/card-shader-reflections)
> **Source Code**: [/src/animations/card-shader-reflections](/src/animations/card-shader-reflections)

## Tags
- `reanimated`
- `skia`

## Description

This is a minimalist card carousel that uses interpolation to create a perspective effect.

The most challenging aspect lies in the CardCanvas component, which handles the shader implementation. The design was inspired by the Trade Republic app.

While the current implementation works, it needs improvement - particularly the shader code, which has to be more readable and maintainable.

## Project Structure

```typescript
src/  ├── components/  │   └── card-carousel/  │       ├── card/  │       │   ├── card.component.tsx       # The star of the show  │       │   ├── card-canvas.component.tsx # Where the magic happens  │       │   ├── card-chip.component.tsx  # That cool chip on your card  │       │   ├── card.shader.ts          # Special effects central  │       │   └── card.styles.ts          # Making it look pretty  │       ├── utils/  │       │   ├── constants.ts            # Our helpful constants  │       │   └── types.ts                # TypeScript goodness  │       ├── card-carousel.tsx           # The main carousel  │       └── card-carousel.styles.ts     # Carousel styling  └── index.tsx                           # Where it all begins
```

GitHubAsk for support

Card Shader Reflections - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
