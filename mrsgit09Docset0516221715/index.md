# Welcome!

This is a test of a method that "converts" documents from MSDN to docs.microsoft.com without creating official markdown. Instead, it uses the HTML created by the GenDox build as inline HTML in markdown files.

This is accomplished by replacing the .htm extension with .md extension.
The document TOCs were generated from the HxT files produced by the build.

## Known Issues
* Glossary bookmarks need to be changed to correct an issue that causes whole terms to be "links".
* Table formatting - easily fixed with custom CSS
* Generated links go to .htm instead of .html
* Extra HTML tags at the bottom of all pages
* Code boxes don't wrap - but do we want them to?