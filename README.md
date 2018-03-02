# PDFJS-Viewer
A library to allow integrating a PDFJS viewer in other pages easily

# Usage

You have to import both PDFJS, and PDFJS-Viewer into your HTML page.

For your convienience, this package has a version of PDFJS under `/build`.

Also, your HTML page needs to have the DOM for the viewer. You can copy/paste the content of `<body>` in `/web/viewer.html`.

Then, you can call `window.PDFViewer(options)`.

`options` is an optional Object argument, which defaults to the following:

```javascript
{
  defaultUrl: DEFAULT_URL, // The document to load upon instantiation
  isViewerEmbedded: false,
  focusPreviewer: true, // Auto-focus the previewer to allow keyboard shortcuts directly after instantiation
  allowPrinting: true, // Show a "Print" button
  allowDownload: true, // Show a "Download" button which downloads the current document
  allowBookmark: true, // Show a "Bookmark" button which gives an URL that reproduces the exact current view. If disabled, hides the button and ignores the URL hash parameters.
  allowUrlQuery: true, // Allow changing the file with URL like `viewer.html?file=foo.pdf`
  allowOpenFile: true // Allow previewer to open new files.
}
```
