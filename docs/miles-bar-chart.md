# Miles Bar Chart

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/miles-bar-chart)
> **Source Code**: [/src/animations/miles-bar-chart](/src/animations/miles-bar-chart)

## Tags
- `reanimated`

## What's This About?

This component creates an interactive bar chart visualization that displays weekly data with smooth horizontal scrolling. The chart synchronizes the scroll position with the displayed data, featuring automatic snapping to weeks and formatted date labels. It handles the complex task of converting animated values to regular state for proper rendering, ensuring smooth transitions between different weeks of data.

## Technical Implementation

The component uses:

- Reanimated scrolling
- Animated reactions
- Date formatting
- Window dimensions
- Scroll synchronization

## Usage

```tsx
// Data structuretype WeekData = {  day: Date;  value: number;}[];
// Component propstype WeeklyChartProps = {  width: number;  height: number;  data: WeekData;};
// Basic usage<WeeklyChart  width={windowWidth}  height={150}  data={weeklyData}/>
// Scrollable container<Animated.ScrollView  horizontal  snapToInterval={windowWidth}  showsHorizontalScrollIndicator={false}  decelerationRate="fast">  {/* Week labels */}  <Text>week of {format(day, 'd MMMM')}</Text></Animated.ScrollView>
```

GitHubAsk for support

Miles Bar Chart - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
