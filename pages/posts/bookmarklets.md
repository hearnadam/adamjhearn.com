---
title: Bookmarklets I Use Daily
date: 2021/05/03
description: The bookmarks that power my workflow.
tag: browser
author: Adam Hearn
---
# Bookmarklets I Use Daily

**Tip: Drag the bookmarklet above the code blocks into your bookmark bar.**

### Sci-Hub

I find myself frequently referencing Sci-Hub, even if the full text is available due to the quality of the paper is generally higher than the free one. This bookmarklet will automatically load paper at a given URL in Sci-Hub. Written by me.

<a href="javascript:(function(){window.location=&quot;https://sci-hub.se/&quot;+window.location})()" title="Sci-Hub Bookmark">Sci-Hub</a>

```javascript
function() {
    window.location = "https://sci-hub.se/" + window.location;
}
```



### Playback Speed

Ever find yourself stuck on an extremely boring or slow  video with no playback controls? This bookmarklet lets you input a speed for the video to be played at. Works with most sites, even youtube. Partially written by me.

<a href="javascript:(function(){Array.from(document.getElementsByTagName(&apos;video&apos;)).forEach(vid=&gt;vid.playbackRate=prompt(&quot;Enter a Playback Speed&quot;))})()" title="Playback Speed Bookmark">Playback Speed</a>

```javascript
function() {
    Array.from(
        document.getElementsByTagName('video'))
        .forEach(vid => vid.playbackRate = prompt("Enter a Playback Speed"));
}
```



### PDF Invert

This bookmarklet is great for reading with less eye fatigue at night. Generally I prefer black text on a white background, but sometimes this is quite useful. Written by a [Hacker News reader](https://news.ycombinator.com/item?id=25180600).

![PDFInvert](/public/images/1/PDFInvert.png1/PDFInvert.png)

<a href="javascript:(function(){viewer.style=&apos;filter: grayscale(1) invert(1) sepia(1) contrast(75%)&apos;})()" title="PDF Inversion Bookmark">PDF Invert</a>

```javascript
function() {
    viewer.style = 'filter: grayscale(1) invert(1) sepia(1) contrast(75%)';
}
```



### Base64 Decode

While online decoding works for most use cases, it is extremely convenient to be able to decode B64 strings offline.

<a href="javascript:(function(){alert(atob(prompt(&quot;Input the Base64 text:&quot;)))})()" title="Base64 Decoder">B64 Decode</a>

```javascript
function() {
    alert(atob(prompt("Input the Base64 text:")));
}
```

