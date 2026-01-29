# 🎥 Multimedia Elements in HTML

HTML allows us to create rich user experiences by embedding images, audio, and video directly into our webpages. 

---

## 🖼️ 1. Images (`<img>`)
The `<img>` tag is an **empty element** (it does not have a closing tag).

```html
<img src="assets/images/movie-poster.jpg" alt="Description of the movie poster" width="500">
```
* **src:** The path to your image file.

* **alt:** Crucial for SEO and Accessibility. It describes the image for screen readers and displays if the image fails to load.

* **width/height:** Attributes used to set the size of the image.

## 🔊 2. Audio (`<audio>`)

**Audio Elements:** The audio elements allow you to add sound to your HTML documents. The audio element supports popular audio formats like mp3, wav, and ogg.

```
 <audio src="CrystalizeThatInnerChild.mp3"></audio>
```

 If you want to see the audio player on the page, then you can add the audio element with the controls attribute:
```
 <audio src="CrystalizeThatInnerChild.mp3" controls></audio>
```

The `controls` attribute enables users to manage audio playback, including adjusting volume, and pausing, or resuming playback. The `controls` attribute is a boolean attribute that can be added to an element to enable built-in playback controls. If omitted, no controls will be shown.

* **`loop Attribute:`** The `loop` attribute is a boolean attribute that makes the audio replay continuously.

```
 <audio
  src="https://cdn.freecodecamp.org/curriculum/js-music-player/can't-stay-down.mp3"
  loop
  controls
></audio>
```

* **`Muted Attribute:`** When present in the audio element, the muted boolean attribute will start the audio in a muted state.

```
  <audio
  src="https://cdn.freecodecamp.org/curriculum/js-music-player/can't-stay-down.mp3"
  loop
  controls
  muted
></audio>
```

* **`Source Element:`** When it comes to audio file types, there are differences in which browsers support which type. To accommodate this, you can use source elements inside the audio element and the browser will select the first source that it understands. Here's an example of using multiple source elements for an audio element:

```
<audio controls>
  <source src="audio.ogg" type="audio/ogg" />
  <source src="audio.wav" type="audio/wav" />
  <source src="audio.mp3" type="audio/mpeg" />
</audio>
```

## 🎞️ 3. Video (`<video>`)
Similar to audio, but for visual media like .mp4 or .webm.

```
<video width="640" height="360" controls poster="preview-image.jpg">
  <source src="assets/video/trailer.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
```
- **Poster:** An image that shows while the video is downloading or until the user hits play.

- **Autoplay / loop / muted:** Additional attributes to control behavior (Note: Many browsers require muted for autoplay to work).

All the attributes we have learned so far are also supported in the video element. Here's an example of using a video element with the loop, controls, and muted attributes:

```
<video
  src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
  loop
  controls
  muted
></video>
```
* **`Poster Attribut`**: If you wanted to display an image while the video is downloading, you can use the `poster` attribute. This attribute is not available for `audio` elements and is unique to the `video` element.

```
<video
  src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
  loop
  controls
  muted
  poster="https://peach.blender.org/wp-content/uploads/title_anouncement.jpg?x11217"
  width="620"
></video>
```



  


