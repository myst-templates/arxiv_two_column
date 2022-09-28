# Changes made during port

A list of changes made when porting the original tex and styles to the Curvenote template format.

- Copied `preprint-template.sty` to the root template folder
- Based `template.tex` on a copy of `preprint-template.tex` shipped in the original
- Using Method A for two column layout
- Added `[-IMPORTS-]` to allow packages and configuration to be loaded
- Removed package includes that are already listed in Curvenote base packages
- Moved any package options up (early as possible) into `\PassOptionsToPackage` commands
  - natbib: numbers, square
  - fontenc: T1
  - hyperref: various!
- Set `hidelinks` option in `template.yml:config.schema = false`
- Inserting data blocks
  - Added Orcid IDs optionally by looping over `doc.authors`
  - Title: `doc.title`
  - Ported Author, affiliation via loop with integer numbering
- Added tagged blocks for `abstract` and `acknowledgments`
- Made `keywords` optional based on `doc.tags`
- Added optional `\usepackage{lipsum}` for testing purposes as example content in original uses it
- Ported ORCID ID Link support on authors
