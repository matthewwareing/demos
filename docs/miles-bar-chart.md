# Miles Bar Chart

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/miles-bar-chart)
> **Source Code**: [/src/animations/miles-bar-chart](/src/animations/miles-bar-chart)

## Tags
- `reanimated`

## Description

Scan to try on your device

## Technical Implementation

- Reanimated scrolling
- Animated reactions
- Date formatting
- Window dimensions
- Scroll synchronization

## Usage

```typescript
// Data structuretype WeekData = {  day: Date;  value: number;}[];
// Component propstype WeeklyChartProps = {  width: number;  height: number;  data: WeekData;};
// Basic usage<WeeklyChart  width={windowWidth}  height={150}  data={weeklyData}/>
// Scrollable container<Animated.ScrollView  horizontal  snapToInterval={windowWidth}  showsHorizontalScrollIndicator={false}  decelerationRate="fast">  {/* Week labels */}  <Text>week of {format(day, 'd MMMM')}</Text></Animated.ScrollView>
```

---

*Documentation extracted from reactiive.io/demos*
