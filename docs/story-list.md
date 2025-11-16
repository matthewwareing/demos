# Story List

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/story-list)
> **Source Code**: [/src/animations/story-list](/src/animations/story-list)

## Tags
- `reanimated`
- `gesture-handler`

## What's This About?

This component creates an interactive story list with smooth scrolling and image display. It features customizable item dimensions, gap spacing, and the number of visible items. The implementation includes image caching, gesture handling, and responsive layout calculations, making it perfect for story viewers, image galleries, or horizontal carousels.

## Technical Implementation

The component uses:

- Gesture handling
- Image caching
- Responsive layout
- Custom scrolling
- Item visibility

## Usage

```tsx
// Basic usage<StoryList />
// Customized story list<StoryList  stories={stories}  pagingEnabled={false}  storyItemDimensions={{    width: windowWidth * 0.7,    height: windowWidth  }}  visibleItems={3}  gap={35}  renderItem={({ image }) => (    <Image      contentFit="cover"      cachePolicy="memory-disk"      style={[        {          borderRadius: 20        },        storyItemDimensions      ]}      source={image}    />  )}/>
// Story data structureconst stories = [  {    image: require('./assets/image_01.png')  },  {    image: require('./assets/image_02.jpg')  }];
// Dimensions calculationconst { width } = useWindowDimensions();const storyItemDimensions = useMemo(() => ({  width: width * 0.7,  height: width}), [width]);
```

GitHubAsk for support

Story List - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
