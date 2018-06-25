# 404 Page
404 error page for GitHub Pages to redirect to any document, including those in sub-folders.

This simple 404.html error page:
- grabs the user provided pathname and any url parameters
- tries to get any document with extension passed into Redirect class
- redirects to that document while adding url parameters (if document exists)
- sits happily with 404 error message if document doesn't exist

## Why?
GitHub Pages nicely redirects to .html and .md pages when the extension isn't provided. It doesn't do the same for files of other extensions like .adoc or .asciidoc. It also can't redirect from root based on documents that exist in sub-folders.

**Example:**

If you have a page at pages/about.html, it would be accessible as:
yoursite.github.io/pages/about.html.

404 Page would let you get to that page with:
yoursite.github.io/about

As a result, you wouldn't need to have all your documents located in root. You could place them all in a /pages/ folder, for example.
