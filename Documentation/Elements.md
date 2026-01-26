In HTML, text formatting is handled by a mix of semantic elements (which tell the browser what the text is) and structural elements (which define how the content is organized).

# **Header Tags:** h1 to h6
There are six heading elements in HTML. The h1 through h6 heading elements are used to signify the importance of content below them. The lower the number, the higher the importance, so h2 elements have less importance than h1 elements.

<html>
  <h1>h1 most important heading element</h1>
<h2>h2 second most important heading element</h2>
<h3>h3 third most important heading element</h3>
<h4>h4 fourth most important heading element</h4>
<h5>h5 fifth most important heading element</h5>
<h6>h6 least important heading element</h6>
</html>


# **The Paragraph Tag: <p>**
This is used for paragraphs on a web page.

  <p>This is a paragraph element.</p>

# **Body Element: <body>**
This element is used to represent the content for the HTML document.
<body>
  <h1>CatPhotoApp</h1>
  <p>This is a paragraph element.</p>
</body>

# **Section Elements:**
This element is used to divide up content into smaller sections.
<section>
  <h2>About Me</h2>
  <p>Hi, I am Remsha Yaseen and I am learning web development.</p>
</section>

# **The Division Tag: <div>**
This element is a generic HTML element that does not hold any semantic meaning. It is used as a generic container to hold other HTML elements.
<div>
  <h1>I am a heading</h1>
  <p>I am a paragraph</p>
</div>

# **Img Elements:**
The img element is used to add images to the web page. The src attribute is used to specify the location for that image. For image elements, it's good practice to include another attribute called the alt attribute. Here's an example of an img element with the src and alt attributes:
<img src="path" alt="Description.">

# **Anchor (a) Elements:**
These elements are used to apply links to a web page.
The href attribute is used to specify where the link should go when the user clicks on it.
<a href="path">text</a>

# **List Elements:**
To create a bulleted list of items you should use the **ul** element with one or more **li** elements nested inside like this:
<ul>
  <li>catnip</li>
  <li>laser pointers</li>
  <li>lasagna</li>
</ul>

To create an ordered list of items you should use the ol element:
<ol>
  <li>flea treatment</li>
  <li>thunder</li>
  <li>other cats</li>
</ol>

# **Emphasis (em) Element:**
This is used to place emphasis on a piece of text.
<p>Cats <em>love</em> lasagna.</p>

# **Strong Importance (strong) Element:**
This element is used to place strong emphasis on text to indicate a sense of urgency and seriousness.
<p>
  <strong>Important:</strong> Before proceeding, make sure to wear your safety goggles.
</p>

# **Figure and Figcaption Elements:**
The figure element is used to group content like images and diagrams. The figcaption element is used to represent a caption for that content inside the figure element.

<figure>
  <img src="path" alt="description">
  <figcaption>Cats <strong>hate</strong> other cats.</figcaption>  
</figure>

# **Main Element:**
This element is used to represent the main content for a web page.
<main>
 content
</main>

# **Footer Element:**
This element is placed at the bottom of the HTML document and usually contains copyright information and other important page links.
<footer>
  <p>
    No Copyright - <a href="path">text</a>
  </p>
</footer>


















