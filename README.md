# 404-page
404 error page for GitHub Pages that tries to redirect to html or md files.

This simple 404.html error page:
- grabs the user provided pathname and any url parameters
- tries to get any .html or .md page based on the path name
- redirects to that page while adding url parameters (if page exists)
- sits happily with 404 error message if page doesn't exist
