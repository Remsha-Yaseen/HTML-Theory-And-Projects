# 📝 HTML Forms
Forms are used to collect user input. Whether it's a login page, a search bar, or a movie review submission, the structure remains the same.

----

## 1. The Form Container `<form>`
The `<form>` tag wraps all input elements. It usually has two important attributes:

* **action:** Where the data is sent (a URL).

* **method:** How the data is sent (usually GET or POST).

## 2. Labels and Inputs: The Perfect Pair

A high-quality form always connects a <label> to its <input>. This is crucial for accessibility; when a user clicks the label, the cursor automatically jumps into the input box.


```html
<label for="username">Username:</label>
<input type="text" id="username" name="user_login">
```

* **The Connection:** The for attribute of the label must match the id of the input.

## 3. Common Input Types
The type attribute changes how the input looks and behaves:

* **text:** Standard one-line box.

* **password:** Masks the characters.

* **email:** Ensures the user enters an "@" symbol.

* **number:** Restricts input to digits.

* **checkbox / radio:** For selecting options.

## 4. Form Validation (Client-Side)

Validation prevents "bad data" from being submitted. You can enforce rules directly in HTML without using JavaScript:

| Attribute | Effect | Example Usage |
| :--- | :---: | :---: |
| required | The field cannot be left empty before submission. | `<input type="text" required>` |
| minlength / maxlength | Sets a specific character limit (useful for passwords or usernames). | `<input type="password" minlength="8">` |
| min / max | Sets numeric boundaries (useful for age or quantity). | `<input type="number" min="1" max="10">` |
| pattern | Uses Regular Expressions (Regex) to enforce specific formats. | `<input type="tel" pattern="[0-9]{3}-[0-9]{3}">` |


