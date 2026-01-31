## 📊 HTML Tables

Tables allow you to arrange data—like text, images, or links—into rows and columns. While we don't use tables for page layouts anymore (we use CSS for that), they are essential for displaying tabular data.

----

**1. The Core Anatomy of a Table**
An HTML table is built using a specific hierarchy of tags. Think of it like a container (the table) holding rows, which then hold individual cells.

* `<table>:` The main container for all table content.
* `<tr>` **(Table Row)**: Defines a horizontal row of cells.
* `<th>` **(Table Header):** Used for the top row to define what the column represents. The text is **bold** and **centered** by default.
* `<td>` **(Table Data):** The standard cell containing the actual information.

**2. Structural Tags (thead, tbody, tfoot)**
For more professional and accessible tables, we divide them into three semantic sections:

* `<thead>:` Wraps the header rows.
* `<tbody>:` Wraps the main content/data of the table.
* `<tfoot>:` Wraps the summary or footer row (e.g., a "Total" line).

 **3. Advanced Attributes: Spanning**
Sometimes a cell needs to take up more than one spot. We use "Spanning" for this:

* `colspan:` Stretches a cell horizontally across multiple columns.
* `rowspan:` Stretches a cell vertically across multiple rows.

💻 **## Code Example:**

```html
<table>
  <thead>
    <tr>
      <th>Project Name</th>
      <th>Status</th>
      <th>Files</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Movie Review</td>
      <td>Completed</td>
      <td>3</td>
    </tr>
    <tr>
      <td>iFrames Study</td>
      <td>In Progress</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
```
