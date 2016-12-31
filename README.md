# extracast-subtitles
Subtitle module used by the [Extracast](https://github.com/dudewheresmycode/Extracast) media player.

**Basic Example**

```javascript
  //pass the element you want the subtitles to be rendered in
  var videoSubtitles = new ecSubtitles(document.getElementById("video-subtitles"));

  //load the subtitles file
  videoSubtitles.load("/subtitles.srt", function(err){
    console.log("Subtitles loaded!")
  });

  video.ontimeupdate = function(){
    //update the playtime
    videoSubtitles.timeupdate(video.currentTime);    
  }
```
