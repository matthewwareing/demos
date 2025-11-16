# Image Cropper

> **Live Demo**: [View on reactiive.io](https://reactiive.io/demos/image-cropper)
> **Source Code**: [/src/animations/image-cropper](/src/animations/image-cropper)

## Tags
- `gesture-handler`
- `skia`

## Description

Scan to try on your device

## Technical Implementation

- Stack navigation
- Modal presentations
- Image manipulation
- Screen transitions
- Dark theme styling

## Usage

```typescript
// Navigation typestype RootStackParamList = {  ImageCropper: undefined;  DetailCroppedImage: {    // Image details  };};
// Basic usage<ImageCropper />;
// Navigation setupconst Stack = createNativeStackNavigator<RootStackParamList>();
<Stack.Navigator  screenOptions={{    presentation: 'modal',    contentStyle: {      backgroundColor: '#000',    },  }}>  <Stack.Screen name="ImageCropper" component={ImageCropperScreen} />  <Stack.Screen name="DetailCroppedImage" component={DetailImageScreen} /></Stack.Navigator>;
```

---

*Documentation extracted from reactiive.io/demos*
