# Uraikus IDE
[Try Here](https://ide.patricktrester.com/)

This IDE runs as a single .html file. Included is the .proj file to modify the editor itself in the editor.

When exporting a .proj file to .html, it will minify and transpile the virtual files into a single file. Any tag that has the "file" attribute, will 
contain the value of such a virutal file. So using a virtual CSS stylesheet, rather than doing a link tag, you would do a style tag with a file attribute.
Though you can still load external resources as you normally would.

```html
<!-- Example CSS Virtual File -->
<style file="design.css"></style>

<!-- Example HTML Virtual File -->
<div file="widget.html"></div>
```
