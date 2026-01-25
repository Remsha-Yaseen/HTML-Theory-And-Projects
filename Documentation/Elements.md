In HTML, text formatting is handled by a mix of semantic elements (which tell the browser what the text is) and structural elements (which define how the content is organized).

# **Header Tags:** h1 to h6
These tags define the hierarchy and importance of headings on a page.
* **Usage:** **(h1)** is the most important (main title), and **(h6)** is the least important (sub-sub-sub-heading).
* **SEO & Accessibility:** Screen readers and search engines use these to understand the structure of your content. You should ideally only have one (h1) per page.
* **Behavior:** They are block-level elements (they start on a new line and take up the full width).

# The Paragraph Tag: <p>
The primary tag for blocks of text.
* **Usage:** Used to wrap sentences and paragraphs.
* **Behavior:** Like headers, (p) is a block-level element. Browsers automatically add a small amount of space (margin) above and below a paragraph to separate it from other content.

 # The Span Tag: <span>
 A generic inline container used for styling specific parts of a text.
**Usage:** Used when you want to change the color, font, or weight of just one word or a phrase inside a paragraph without breaking the line.
**Behavior:** It is an inline element; it does not start on a new line and only takes up as much width as necessary.
_Example:_ <p>This is <span style="color:red;">important</span> text.</p>

# The Division Tag: <div>
The most common container in web development, used to group other elements together.
**Usage:** It has no semantic meaning (it doesn't tell the browser if the content is a header or a paragraph). It is used strictly for styling or layout purposes (e.g., creating a sidebar or a wrapper).
**Behavior:** It is a block-level element.
