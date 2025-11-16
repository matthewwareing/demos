# Demos ✨

An ongoing collection of React Native animations crafted with Reanimated, Gesture Handler, and Skia.

Browse all demos at [reactiive.io/demos](https://reactiive.io/demos).

## Documentation

Comprehensive documentation for all 106 animations is available in the [/docs](/docs) folder. Each animation includes:
- Detailed descriptions and behavior explanations
- Usage examples with code snippets
- Key features and technical implementation details
- Links to live demos and source code

[Browse all animation docs →](/docs)

## Highlights

Demos 2024 - Rewind 👇

https://github.com/user-attachments/assets/47c8fb6d-6810-444f-a92e-589ffae84778

Demos 2023 - Rewind: [Twitter Post](https://x.com/reactiive_/status/1740314524501078359)

## Roadmap

This project is a work in progress (almost by definition). Here are the current priorities:

- [x] Remove deprecated APIs: runOnJS and runOnUI should now be imported from react-native-worklets
- [x] Drawer Navigation: currently the navigation is quite unintuitive and needs to be improved.
- [x] Ensure consistent haptics support (use [pressto](https://github.com/enzomanuelmangano/pressto) whenever possible)
- [ ] Optimize performance in Shaders demos
- [x] Feedback screen on Shake Detection
- [x] [TestFlight Release](https://testflight.apple.com/join/uB9PQHuT)
- [ ] Android Release (starting with App Tester / Firebase Distribution)

## Quick Start

This is an Expo Go project. To get started:

```bash
bun install
bun ios     # for iOS
# or
bun android # for Android
```

## Project Layout

```
src/
├── animations/   # Where the magic happens
└── navigation/   # app navigation utils and hooks
docs/             # Animation documentation and explainers
```

## Sponsors

If you find these animations helpful, consider supporting the project:

- 💖 [GitHub Sponsors](https://github.com/sponsors/enzomanuelmangano)
- ✨ [Demos](https://reactiive.io/demos)
- 🎓 **Learn to build these animations**: Check out my course at [reanimate.dev](https://reanimate.dev). Dive deep into the world of React Native animations with this course, designed to guide you from the basics to advanced techniques

Your support helps maintain this project and support my open-source work!

## License

This project is licensed under a custom Software License Agreement. See [LICENSE.md](./LICENSE.md) for details.

**Key points:**

- ✅ Free for everyone (individuals and companies)
- ✅ Can use in commercial projects
- ✅ Can modify and customize for your needs
- ❌ Cannot resell or redistribute the code
- ❌ Cannot create competing animation libraries
