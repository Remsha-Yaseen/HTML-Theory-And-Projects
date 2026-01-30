# 🖼️ iFrames in HTML

The `<iframe>` (Inline Frame) tag is used to embed another document or website within the current HTML document. It essentially creates a "window" to another piece of content.

---

## 1. Basic Syntax
The most common use for an `iframe` is embedding a YouTube video or an interactive map.

```html
<iframe src="[https://www.wikipedia.org](https://www.wikipedia.org)" width="100%" height="500px" title="Wikipedia Frame">
  <p>Your browser does not support iframes.</p>
</iframe>
```

**Key Attributes:**

+ **src:** The URL of the page or file you want to embed.
* **width & height:** Sets the size of the "window."
* **title:** (Very Important) Describes the content for screen readers. This is a must-have for accessibility.
* **frameborder:** (Old school) Usually set to "0" to remove the border around the frame.

You can include the allowfullscreen attribute which allows the user to display the iframe in full screen mode.

```html
<iframe
  src="video-url"
  width="width-value"
  height="height-value"
  allowfullscreen
></iframe>
```

## 2. Embedding YouTube Videos

YouTube provides a specific "Embed" code. You don't use the standard <video> tag for YouTube; you use an iframe.

```html
<iframe 
  width="560" 
  height="315" 
  src="[https://www.youtube.com/embed/dQw4w9WgXcQ](https://www.youtube.com/embed/dQw4w9WgXcQ)" 
  title="YouTube video player" 
  allowfullscreen>
</iframe>
```
* allowfullscreen: Allows the user to expand the video to their whole screen.


### 🛡️ **Advanced iFrame Attributes: Permissions & Privacy**

Beyond just the src, modern iFrames use specific attributes to manage security and hardware access.

**`The allow Attribute (Permission List)`**
The **allow** attribute acts as a feature policy. It tells the browser exactly which device features the embedded content is permitted to use.

* `accelerometer:` Grants access to motion sensors to detect device tilting and rotation (essential for gaming or 360° views).
* `autoplay:` Allows media content to start playing automatically upon page load.
* `clipboard-write:` Permits the iFrame to copy data directly to the user's clipboard.
* `encrypted-media:` Enables the use of "Encrypted Media Extensions" to protect copyrighted video content from being easily copied.
* `gyroscope:` Grants access to the device’s orientation sensors (often used alongside the accelerometer).
* `web-share:` Allows the iFrame to trigger the device’s native "Share" menu (so users can share the content directly to their apps).

**`The referrerpolicy Attribute (Privacy Control)`**

This attribute is a "rule book" for privacy. It determines how much information your website shares with the target website when the iFrame connects.

**Recommended Setting:** `strict-origin-when-cross-origin`

+ **Same-Site:** It shares the full URL of your page if the iFrame is from your own site.
+ **Cross-Origin:** It only shares your site name (domain) if the iFrame is from a different website.
+ **Insecure Sites:** It shares nothing if your site is secure (`https`) and the iFrame source is not (`http`).

**Why use this?** It protects your users' privacy by not leaking the specific page paths they are visiting to third-party trackers.

```html
<iframe 
  src="https://www.youtube.com/embed/example" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; web-share" 
  referrerpolicy="strict-origin-when-cross-origin" 
  allowfullscreen>
</iframe>
```
