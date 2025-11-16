# Swipe Cards

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/swipe-cards)
> **Source Code**: [/src/animations/swipe-cards](/src/animations/swipe-cards)

## Tags
- `reanimated`
- `gesture-handler`
- `skia`

## What's This About?

This component creates an interactive card swipe interface similar to dating apps. It features smooth swipe animations, like/dislike actions, and a reset function. The implementation includes gesture handling for card swipes, fade animations for card transitions, and control buttons for manual actions, making it perfect for any interface requiring card-based decision making.

## Technical Implementation

The component uses:

- Swipe gestures
- Card stacking
- Action buttons
- Fade animations
- State tracking

## Usage

```tsx
// Basic usage<SwipeCards />
// Swipeable card<SwipeableCard  index={index}  activeIndex={activeIndex}  image={image}  ref={cardRef}  onSwipeRight={() => {    liked.current += 1;  }}  onSwipeLeft={() => {    disliked.current += 1;  }}/>
// Control buttons<View style={styles.buttonsContainer}>  <PressableScale    style={styles.button}    onPress={swipeLeft}  >    <AntDesign name="close" size={32} color="white" />  </PressableScale>
  <PressableScale    style={styles.button}    onPress={reset}  >    <AntDesign name="reload1" size={24} color="white" />  </PressableScale>
  <PressableScale    style={styles.button}    onPress={swipeRight}  >    <AntDesign name="heart" size={32} color="white" />  </PressableScale></View>
// Swipe controls hookconst {  activeIndex,  refs,  swipeRight,  swipeLeft,  reset} = useSwipeControls();
```

GitHubAsk for support

Swipe Cards - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
