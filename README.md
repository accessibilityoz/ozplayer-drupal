OzPlayer for Drupal
===================

This is a 'custom' plugin for Drupal. It provides a filter to insert videos for
playback with the free version of OzPlayer.

To use, add the 'ozplayer' directory to sites/all/modules and enable the module.
Then add the filter to appropriate node types.

To display a video insert the following in a page:

    [ozplayer|mp4://example.com/some/video.mp4|webm://example.com/some/video.webm|captions:/some/path/captions.vtt|transcript:/some/path/transcript.vtt|mp3://example.com/some/video.mp3|ogg://example.com/some/video.ogg]

Alternately, if you want to embed a YouTube video, skip the 'mp4' and 'webm' arguments
and instead use 'yt://youtube.com/watch?v=xxxxxxxx'.

Note that you can't use a protocol specifier (e.g., 'http://') on these URLs as the
colon is being used to split keywords and values. Generally this will be fine.
