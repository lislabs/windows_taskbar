<h1 align="center"><a href="https://github.com/alexmercerind/windows_taskbar">windows_taskbar</a></h1>
<h4 align="center">Flutter plugin serving utilities related to Windows taskbar 💙</h4>

## Install

```yaml
dependencies: 
  windows_taskbar: ^1.0.0
```

## Demo

Checkout the example Flutter application [here](https://github.com/alexmercerind/windows_taskbar/blob/master/example/lib/main.dart).

![](https://github.com/alexmercerind/windows_taskbar/blob/assets/bMebejv57F.gif)
![](https://github.com/alexmercerind/windows_taskbar/blob/assets/OdzgD1yqEO.gif)


## Documentation

**Set thumbnail toolbar**

```dart
WindowsTaskbar.setThumbnailToolbar(
  [
  ThumbnailToolbarButton(
    ThumbnailToolbarAssetIcon('assets/camera.ico'),
      'Turn On Camera',
      () {},
    ),
    ThumbnailToolbarButton(
      ThumbnailToolbarAssetIcon('assets/microphone.ico'),
      'Mute',
      () {},
      mode: ThumbnailToolbarButtonMode.disabled | ThumbnailToolbarButtonMode.dismissionClick,
    ),
    ThumbnailToolbarButton(
      ThumbnailToolbarAssetIcon('assets/end_call.ico'),
      'Disconnect',
      () {},
    ),
  ],
);
```

**Clear thumbnail toolbar**

```dart
WindowsTaskbar.clearThumbnailToolbar();
```

**Set progress mode**

```dart
WindowsTaskbar.setProgressMode(TaskbarProgressMode.indeterminate);
```

**Set progress**

```dart
WindowsTaskbar.setProgress(69, 100);
```

**Set thumbnail tooltip**

```dart
WindowsTaskbar.setThumbnailTooltip('Awesome Flutter window.');
```

**Flash windows taskbar app icon**

```dart
WindowsTaskbar.flashTaskbarAppIcon(
  mode: TaskbarFlashMode.all | TaskbarFlashMode.timernofg,
  timeout: const Duration(milliseconds: 500),
);
```

**Stop flashing windows taskbar app icon**

```dart
WindowsTaskbar.stopFlashingTaskbarAppIcon();
```

**Set overlay icon (a badge)**

```dart
WindowsTaskbar.setOverlayIcon(icon: 'res/circle.ico', altTooltip: 'Alternative tooltip for badge');
```

**Remove overlay icon (a badge)**

```dart
WindowsTaskbar.resetOverlayIcon();
```

## License

Copyright © 2021 & 2022, Hitesh Kumar Saini <<saini123hitesh@gmail.com>>

This library & all the work in this repository is under MIT license that can be found in the LICENSE file.


## Donate 

Consider donating me at https://www.paypal.me/alexmercerind if you like the plugin. So that I can atleast pay my internet bill.
