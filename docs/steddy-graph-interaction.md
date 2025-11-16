# Steddy Graph Interaction

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/steddy-graph-interaction)
> **Source Code**: [/src/animations/steddy-graph-interaction](/src/animations/steddy-graph-interaction)

## Tags
- `reanimated`
- `skia`

## What's This About?

This component creates an interactive graph visualization with a segmented control for different difficulty levels. It features smooth transitions between different score sets, customizable graph dimensions, and responsive layout. The implementation includes difficulty selection controls and a dynamic graph display, making it perfect for data visualization with interactive controls.

## Technical Implementation

The component uses:

- Segmented controls
- Graph rendering
- Score mapping
- Window dimensions
- Custom fonts

## Usage

```tsx
// Basic usage<SteddyGraphInteraction />
// Graph component<Graph  scores={scores}  canvasHeight={200}  canvasWidth={windowWidth}  padding={50}  maxValue={100}  lineScore={70}  style={{ marginTop: 20 }}/>
// Segmented control<SegmentedControl  data={['Light', 'Standard', 'Pro']}  onPress={(item) => {    setSelectedDifficulty(item);  }}  width={windowWidth - 30}  height={56}  selected={difficulty}/>
// Score mappingconst ScoringMap = {  Light: LIGHT_GRAPH_SCORES,  Standard: STANDARD_GRAPH_SCORES,  Pro: PRO_GRAPH_SCORES};
// Window dimensionsconst { width: windowWidth } = useWindowDimensions();
// Score calculationconst scores = useMemo(() => {  return ScoringMap[difficulty];}, [difficulty]);
```

GitHubAsk for support

Steddy Graph Interaction - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
