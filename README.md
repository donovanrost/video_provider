# Video Provider

This library enables you to extract mp4 videos from various video providers. Currently supported:

- Imgur
- Gfycat

More will follow, feel free to make pull requests or raise issues with examples.

## Usage

A simple usage example:

```dart
import 'package:video_provider/src/video.dart';
import 'package:video_provider/video_provider.dart';

main() {
  List<Video> potentialUris = VideoProvider
      .fromUri(Uri.parse("https://i.imgur.com/example.gifv"))
      .getVideos();

  // prints https://i.imgur.com/example.mp4
  for(var video in potentialUris)
    print(video.uri);
  
}
```

## Features and bugs

Please file feature requests and bugs at the [issue tracker][tracker].

[tracker]: https://github.com/StefanLobbenmeier/video_provider/issues
