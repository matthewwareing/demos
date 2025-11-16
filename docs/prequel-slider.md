# Prequel Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/prequel-slider)
> **Source Code**: [/src/animations/prequel-slider](/src/animations/prequel-slider)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## What's This About?

This component creates a sophisticated image editing interface with a custom slider control and visual transitions. It features a draggable slider that controls both a circular progress indicator and image transition effects. The component includes smooth color interpolation, safe area handling, and WebGL-based image transitions, making it suitable for photo editing applications.

## Technical Implementation

The component uses:

- Skia for rendering
- WebGL transitions
- Color interpolation
- Gesture handling
- Progress indicators

## Usage

```tsx
// Basic usage<PrequelSlider />
// Image editor with transitions<ImageEditor  width={imageEditorWidth}  height={imageEditorHeight}  glEffect={ButterflyWaveScrawlerGL}  image={demoImage}  progress={progressPercentage}  style={{    borderRadius: 10,    overflow: 'hidden',    borderCurve: 'continuous'  }}/>
// Draggable slider configuration<DraggableSlider  linesAmount={50}  spacePerLine={10}  maxLineHeight={12}  minLineHeight={5}  bigLineIndexOffset={10}  lineWidth={2}  snapEach={1}  scrollableAreaHeight={60}  onProgressChange={(progress) => {    // Handle progress updates  }}/>
```

GitHubAsk for support

Prequel Slider - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
