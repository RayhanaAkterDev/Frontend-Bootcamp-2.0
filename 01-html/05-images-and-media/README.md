# HTML Images and Media

> Tags: html-img-media  
> _Purpose:_ Understand the core concepts of using images, audio, video, and embedded content in HTML.

---

## My understanding

### Image section

- Used `figure` and `figcaption` to wrap images with descriptive captions.
- The `<img>` tag includes several useful attributes:
  - `width` – sets the width of the image.
  - `height` – sets the height of the image.
  - `loading="lazy"` – defers loading for large images to improve performance.
  - `src` – defines the image source path (online or local).
  - `alt` – provides alternative text if the image fails to load.
  - `title` – adds a tooltip when the user hovers over the image.
- Images can be displayed using:
  - **Absolute path** (online image).  
    _Example:_ `src="https://images.unsplash.com/..."`  
  - **Relative path** (local image).  
    _Example:_ `src="../../00-assets/images/dog-image.jpeg"`

---

### Audio section

- Used the `<audio>` element to embed sound files.
- Inside it, a `<source>` tag defines the audio file and its format:
  - `src` – specifies the path to the audio file.
  - `type` – describes the file type (e.g., `"audio/mp3"`).
- Key attributes:
  - `controls` – displays the default audio player UI.
  - `autoplay` – plays the audio automatically on page load.
- Included fallback text inside the tag in case the browser does not support audio.

---

### Video section

- Used the `<video>` element to embed video content.
- Inside it, a `<source>` tag defines the video file and its format:
  - `src` – specifies the path to the video file.
  - `type` – defines the format (e.g., `"video/mp4"`).
- Key attributes:
  - `controls` – displays the default video controls.
  - `autoplay` – starts video playback automatically.
  - `loop` – restarts the video when it ends.
  - `muted` – mutes the video by default (required for autoplay).
  - `width` – defines the display width of the video player.

---

### Iframe section

- Used the `<iframe>` tag to embed external content like YouTube videos.
- Important attributes:
  - `src` – specifies the embedded URL.
  - `width` / `height` – define the iframe's visible size.
  - `allowfullscreen` – allows fullscreen mode.
  - `loading="lazy"` – delays loading to improve performance.
  - `referrerpolicy` – manages what referrer data is shared.

---

> Note:
>
> - Always use `alt` text for better accessibility and SEO.
> - Avoid autoplay unless the media is muted (especially important for user experience).
> - Wrap visual content with semantic tags like `figure` and `figcaption` where appropriate.
> - Use `loading="lazy"` for large images and iframes to optimize page speed.
> - Prefer `<source>` inside `<audio>` and `<video>` for better format handling across browsers.

---

### Code links

- [Template code](01-template.html)
- [Exercise code](02-exercise.html)

---
