# Swipe Cards

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/swipe-cards)
> **Source Code**: [/src/animations/swipe-cards](/src/animations/swipe-cards)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Swipe gestures
- Card stacking
- Action buttons
- Fade animations
- State tracking

## Usage

```typescript
// Basic usage<SwipeCards />
// Swipeable card<SwipeableCard  index={index}  activeIndex={activeIndex}  image={image}  ref={cardRef}  onSwipeRight={() => {    liked.current += 1;  }}  onSwipeLeft={() => {    disliked.current += 1;  }}/>
// Control buttons<View style={styles.buttonsContainer}>  <PressableScale    style={styles.button}    onPress={swipeLeft}  >    <AntDesign name="close" size={32} color="white" />  </PressableScale>
  <PressableScale    style={styles.button}    onPress={reset}  >    <AntDesign name="reload1" size={24} color="white" />  </PressableScale>
  <PressableScale    style={styles.button}    onPress={swipeRight}  >    <AntDesign name="heart" size={32} color="white" />  </PressableScale></View>
// Swipe controls hookconst {  activeIndex,  refs,  swipeRight,  swipeLeft,  reset} = useSwipeControls();
```

---

*Documentation extracted from reactiive.io/demos*
