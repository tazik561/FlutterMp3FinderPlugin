# flutter_mp3_finder

A flutter plugin to get all Mp3 files and it's information like [Path, Album, Album Image, Artist, DateAdded, Duration and Size, ] from phone storage as json format.

``` dart
dependencies:
 flutter_mp3_finder: ^0.1.0
```

Sample Code
```dart 

    try {
      var mp3String = await FlutterMp3Finder.scanDeviceForMp3Files;
      _models = DataModel.fromJson(json.decode(mp3String));
    } on Exception catch (e) {
      print(e);
    }

```

> Only for Android.

