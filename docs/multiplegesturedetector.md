## Multiple gesture detector

If you need to wrap `BetterPlayer` widget with `GestureDetector` widget then you need to use `BetterPlayerMultipleGestureDetector`.

```dart
BetterPlayerMultipleGestureDetector(
            child: AspectRatio(
              aspectRatio: 16 / 9,
              child: BetterPlayer(controller: _betterPlayerController),
            ),
            onTap: () {
              debugPrint("Tap!");
            },
          ),
```

Supported gestures:
* `onTap`
* `onDoubleTap`
* `onLongPress`

If you need to have different gestures than mentioned above then you can use default `GestureDetector`.