# Story List

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/story-list)
> **Source Code**: [/src/animations/story-list](/src/animations/story-list)

## Tags
- `reanimated`
- `gesture-handler`

## Description

Scan to try on your device

## Technical Implementation

- Gesture handling
- Image caching
- Responsive layout
- Custom scrolling
- Item visibility

## Usage

```typescript
// Basic usage<StoryList />
// Customized story list<StoryList  stories={stories}  pagingEnabled={false}  storyItemDimensions={{    width: windowWidth * 0.7,    height: windowWidth  }}  visibleItems={3}  gap={35}  renderItem={({ image }) => (    <Image      contentFit="cover"      cachePolicy="memory-disk"      style={[        {          borderRadius: 20        },        storyItemDimensions      ]}      source={image}    />  )}/>
// Story data structureconst stories = [  {    image: require('./assets/image_01.png')  },  {    image: require('./assets/image_02.jpg')  }];
// Dimensions calculationconst { width } = useWindowDimensions();const storyItemDimensions = useMemo(() => ({  width: width * 0.7,  height: width}), [width]);
```

---

*Documentation extracted from reactiive.io/demos*
