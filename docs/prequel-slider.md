# Prequel Slider

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/prequel-slider)
> **Source Code**: [/src/animations/prequel-slider](/src/animations/prequel-slider)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Skia for rendering
- WebGL transitions
- Color interpolation
- Gesture handling
- Progress indicators

## Usage

```typescript
// Basic usage<PrequelSlider />
// Image editor with transitions<ImageEditor  width={imageEditorWidth}  height={imageEditorHeight}  glEffect={ButterflyWaveScrawlerGL}  image={demoImage}  progress={progressPercentage}  style={{    borderRadius: 10,    overflow: 'hidden',    borderCurve: 'continuous'  }}/>
// Draggable slider configuration<DraggableSlider  linesAmount={50}  spacePerLine={10}  maxLineHeight={12}  minLineHeight={5}  bigLineIndexOffset={10}  lineWidth={2}  snapEach={1}  scrollableAreaHeight={60}  onProgressChange={(progress) => {    // Handle progress updates  }}/>
```

---

*Documentation extracted from reactiive.io/demos*
