# 🔗 Links and Anchors in HTML

The anchor tag `<a>` is used to create hyperlinks. Links are the most important part of the web because they allow users to navigate between pages and websites.

---

## 1. External Links
Used to link to a website outside of your project (like Google or GitHub).

```html
<a href="https://www.google.com" target="_blank">Visit Google</a>
```
* href: The destination URL.
* target="_blank": This is a best practice; it opens the link in a new tab.

## 2. Internal (Relative) Links:
Used to link to another file inside your own project folders. This is very important for your GitHub repository structure!
* **Link to a file in the same folder:**
```html
<a href="Boilerplate.md">View Boilerplate Notes</a>
```
* **Link to a file inside a different folder:**
```html
<a href="../Projects/index.html">View My Project</a>
```
(The ../ tells the browser to go "up" one folder level.)

## 3. Anchor Links (Jump Links):
Used to jump to a specific section on the same page.
```html
<h2 id="contact-section">Contact Me</h2>

<a href="#contact-section">Jump to Contact</a>
```

## 4. Email and Phone Links:
You can create links that automatically open the user's email app or dial a phone number.
```html
<a href="mailto:example@email.com">Send me an Email</a>
<a href="tel:+123456789">Call Me</a>
```
