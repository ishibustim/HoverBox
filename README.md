# HoverBox
Clean and modern tooltips

# Usage
Include the following lines in your `<head>`:  
```html
<link rel="stylesheet" type="text/css" href="HoverBox.css" />
<script type="text/javascript" src="HoverBox.js" defer></script>
```

To indicate that an element can display a HoverBox, add the class `HBHasHoverBox` to the element.
The title for the HoverBox can be set by setting the value of the `HBTitle` attribute.
There are a couple options for setting the content of the HoverBox.
1) Set the value of the `HBBody` attribute
2) Set the value of the `HBBodyElem` attribute to the ID of a template element (including the `#`)

If using the second option, you may add the class `HBTemplate` to the template

Examples:
```html
<div class="HBHasHoverBox" HBTitle="Sample HoverBox" HBBody="This is a sample HoverBox.">Hover here to see a sample HoverBox</div>
```

```html
<div class="HBHasHoverBox" HBTitle="Sample Template HoverBox" HBBodyElem="#Template">Hover here to see a sample HoverBox using a template element</div>

<div id="Template" class="HBTemplate">
    HoverBox bodies support HTML tags, such as <strong>bold</strong> and <em>italics</em>.
</div>
```

# Requirements
- JQuery
