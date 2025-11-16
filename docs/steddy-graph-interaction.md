# Steddy Graph Interaction

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/steddy-graph-interaction)
> **Source Code**: [/src/animations/steddy-graph-interaction](/src/animations/steddy-graph-interaction)

## Tags
- `reanimated`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Segmented controls
- Graph rendering
- Score mapping
- Window dimensions
- Custom fonts

## Usage

```typescript
// Basic usage<SteddyGraphInteraction />
// Graph component<Graph  scores={scores}  canvasHeight={200}  canvasWidth={windowWidth}  padding={50}  maxValue={100}  lineScore={70}  style={{ marginTop: 20 }}/>
// Segmented control<SegmentedControl  data={['Light', 'Standard', 'Pro']}  onPress={(item) => {    setSelectedDifficulty(item);  }}  width={windowWidth - 30}  height={56}  selected={difficulty}/>
// Score mappingconst ScoringMap = {  Light: LIGHT_GRAPH_SCORES,  Standard: STANDARD_GRAPH_SCORES,  Pro: PRO_GRAPH_SCORES};
// Window dimensionsconst { width: windowWidth } = useWindowDimensions();
// Score calculationconst scores = useMemo(() => {  return ScoringMap[difficulty];}, [difficulty]);
```

---

*Documentation extracted from reactiive.io/demos*
