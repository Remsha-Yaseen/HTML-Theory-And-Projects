# 🔍 Understanding HTML Meta Tags

Meta tags are snippets of text that describe a page's content. They don't appear on the page itself, but only in the page's code (the `<head>` section). They are crucial for **SEO** (Search Engine Optimization) and **User Experience**.

---

## 📱 The Viewport Meta Tag
This is arguably the most important tag for modern web development. It ensures your website is **Responsive** (looks good on mobile).


<meta name="viewport" content="width=device-width, initial-scale=1.0">

width=device-width: Sets the width of the page to follow the screen-width of the device.

initial-scale=1.0: Sets the initial zoom level when the page is first loaded.

📈 SEO Meta Tags
These tags tell search engines what your site is about so they can show it to the right people.

1. Description
This text often appears in Google search results.


<meta name="description" content="A beginner's guide to learning HTML and building web projects.">

2. Keywords
(Less important now, but still used) To list topics covered.)

<meta name="keywords" content="HTML, Web Development, Beginner, Documentation">

3. Author
To define who created the page.

<meta name="author" content="Your Name">

🛠️ Character Encoding
To make sure special characters and emojis display correctly, we always use UTF-8.
<meta charset="UTF-8">

🖼️ Social Media (Open Graph) Tags
Have you ever shared a link on WhatsApp or LinkedIn and a nice image/title appeared? That's done using og: tags.

<meta property="og:title" content="My HTML Journey">
<meta property="og:description" content="Check out my progress on GitHub!">
<meta property="og:image" content="link-to-your-preview-image.jpg">

