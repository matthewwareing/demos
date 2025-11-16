# Radar Chart

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/radar-chart)
> **Source Code**: [/src/animations/radar-chart](/src/animations/radar-chart)

## Tags
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Skia rendering
- Custom fonts
- Dynamic data generation
- Grid visualization
- Multiple data layers

## Usage

```typescript
// Data structuretype RadarKeys = 'Checkmate' | 'Deflection' | 'Endgame' | 'Fork' | 'Sacrifice';type RadarDataType = Array<{  color: string;  values: Record<RadarKeys, number>;}>;
// Generate random dataconst data = [  {    color: 'rgba(255,255,0,0.2)',    values: {      Checkmate: 1,      Deflection: 0.6,      Endgame: 0.1,      Fork: 0.1,      Sacrifice: 0.5,    },  },  {    color: 'rgba(0,255,255,0.3)',    values: {      Checkmate: 0.2,      Deflection: 0.1,      Endgame: 0.5,      Fork: 0.9,      Sacrifice: 0.8,    },  },];
// Basic usage<RadarChart  data={data}  showGrid={true}  font={font}  internalLayers={5}  strokeWidth={2}  strokeColor="rgba(255,255,255,0.5)"  style={{ width: width, aspectRatio: 1 }}/>;
```

---

*Documentation extracted from reactiive.io/demos*
