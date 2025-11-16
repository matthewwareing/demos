# Expandable Mini Player

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/expandable-mini-player)
> **Source Code**: [/src/animations/expandable-mini-player](/src/animations/expandable-mini-player)

## Tags
- `reanimated`

## Description

Scan to try on your device

## What's This About?

- Transitions between mini and full view
- Shows track information
- Includes playback controls
- Handles gesture interactions
- Maintains state during transitions

## Usage

```typescript
type MiniPlayerProps = {  track: {    title: string;    artist: string;    artwork: string;  };  isPlaying?: boolean;  onPlayPause?: () => void;};
// Basic usage<ExpandableMiniPlayer  track={{    title: 'Track Name',    artist: 'Artist Name',    artwork: 'artwork-url',  }}  isPlaying={false}  onPlayPause={() => {    // Handle play/pause  }}/>;
```

---

*Documentation extracted from reactiive.io/demos*
