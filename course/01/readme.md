# Document & DOM

- [`document`](https://developer.mozilla.org/en-US/docs/Web/API/Document)

> The `Document` interface represents any web page loaded in the browser and serves as an entry point into the web page's content, which is the DOM tree.

Any web page is a `document`. It has all the `elements` inside it that make up the web page.

- [Document Object Model (DOM)](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)

> The `Document Object Model` (`DOM`) connects web pages to programming languages by representing the structure of a document.

`DOM` is the API that connects a `document` (web page) to JavaScript.

- [`document.querySelector()`](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)

> The Document method querySelector() returns the first Element within the document that matches the specified selector, or group of selectors. If no matches are found, null is returned.

Using `querySelector()` you can select any DOM element and do stuff to it with JavaScript.

```js
element = document.querySelector(selectors);
```

- `selectors` This string must be a valid CSS selector string.

## Final Code

The final code can be found in the [`index.html`](./index.html) file.

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Learn React with Awais</title>
	</head>
	<body>
		<div id="root"></div>
		<script src="script.js" type="text/javascript"></script>
	</body>
</html>
```

```js
// 1. Access the `root` element.
const root = document.querySelector('#root');

// 2. Append a heading to it.
const heading = document.createElement('h1');

heading.textContent = 'Learn React with Awais';
root.appendChild(heading);
```

Use your code for good.
