# docfx v3 website example

Example website for docfx v3 which is using docfx-jekyll branch updates.

## Experimental features

- ✅ Allow html pages
- ✅ Allow html layouts
- ✅ Allow html includes
- ✅ Render liquid syntax in markdown and html pages
- ✅ Add Blog page and list posts
- ⌛ ToDo: Add Paginator

## How to install

1. Clone **docfx v3** experimental branch from https://github.com/VaclavElias/docfx/tree/jekyll
    - Compare with upstream https://github.com/dotnet/docfx/compare/v3...VaclavElias:jekyll?expand=1
    - Change the build location in the ```docfx.csproj```, currently it is in ```D:\docfx``` for the testing purpose
    - Build the project
1. Clone template experimental branch https://github.com/VaclavElias/template/tree/jekyll
    - Compare with upstream https://github.com/docascode/template/compare/main...VaclavElias:template:jekyll
    - This template is in VS Solution so we can have scss compilation available and use any VS extensions
    - Extra files added.. compilerconfig.json for scss compilation through VS extension
1. Clone docfx website https://github.com/VaclavElias/docfx-website
    - If needed, update the above template location in the ```docfx.yml``` file
    - Alternatively, you can create your new docfx project/website ```docfx new Conceptual``` and use some of the above website files as example

## How to use

Make any updates you would like. Build with `docfx build` and test with `docfx serve`.

You might need to use whole path to `docfx.exe` if needed.


## Summary
||docfx v3 branch| docfx v3 jekyll branch|
|---|
|Layout|*.liquid|*.liquid<br> *.html
|Includes|*.liquid|*.liquid<br> *.html
|Page|*.md<br> *.yml|*.md (+ liquid content)<br> *.html (+ liquid content)<br> *.yml
|Blog|not available|/blog/index.html access to all pages `page.site.pages`

