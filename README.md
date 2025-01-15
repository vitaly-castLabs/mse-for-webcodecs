# MSE-for-WebCodecs demo / test bed
The [Media Source Extensions API (MSE)](https://www.w3.org/TR/media-source/) requires applications to provide fragments of containerized media
(such as fragmented MP4, WebM) to be able to buffer and play that media. If the application already has the media in a parsed and structured form,
it can cost extra latency and code complexity to package that media into a container and feed it to MSE.

As the web platform is evolving to give applications lower-level abstractions for efficiently encoding and decoding media via the
[WebCodecs API](https://github.com/WICG/web-codecs), MSE can use WebCodec's media structures to let applications more efficiently feed their media to MSE.

More info here: [MSE-for-WebCodecs explainer](https://github.com/wolenetz/mse-for-webcodecs/blob/main/explainer.md)

## Extra resources
[Chrome implementation tracker](https://issues.chromium.org/issues/40155657)\
[WPT demo](https://wpt.live/media-source/mse-for-webcodecs/tentative/mediasource-encrypted-webcodecs-appendencodedchunks-play.https.html)\
[EME-for-WebCodecs](https://github.com/vitaly-castLabs/eme-for-webcodecs) - same code, but with encryption and EME on top
