# Image Cropper

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/image-cropper)
> **Source Code**: [/src/animations/image-cropper](/src/animations/image-cropper)

## Tags
- `gesture-handler`
- `skia`

## What's This About?

This component provides a sophisticated image cropping interface that allows users to select and adjust portions of images. The component features a modal-based navigation flow where users can crop an image and then view the cropped result in detail. The interface is designed with a dark theme and smooth transitions between screens, making it ideal for photo editing applications.

## Technical Implementation

The component uses:

- Stack navigation
- Modal presentations
- Image manipulation
- Screen transitions
- Dark theme styling

## Usage

```tsx
// Navigation typestype RootStackParamList = {  ImageCropper: undefined;  DetailCroppedImage: {    // Image details  };};
// Basic usage<ImageCropper />;
// Navigation setupconst Stack = createNativeStackNavigator<RootStackParamList>();
<Stack.Navigator  screenOptions={{    presentation: 'modal',    contentStyle: {      backgroundColor: '#000',    },  }}>  <Stack.Screen name="ImageCropper" component={ImageCropperScreen} />  <Stack.Screen name="DetailCroppedImage" component={DetailImageScreen} /></Stack.Navigator>;
```

GitHubAsk for support

Image Cropper - FeedbackShare Your ThoughtsI value a lot your feedback! Help me improve by sharing your thoughts, suggestions, or reporting any issues you encounter. If you need assistance, send me an email at hello@reactiive.ioSend Feedback

---

*Documentation extracted from reactiive.io/demos*
