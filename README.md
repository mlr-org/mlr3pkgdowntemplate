
# mlr3pkgdowntemplate

pkgdown template files for all mlr* related packages.

# Changes to original pkgdown templates

All custom changes live in `inst/pkgdown/css/extra.css`

## Changes to `pkgdown.css`

l.125:   `height: 16px;` -> otherwise the orcid icon is oversized

## Changes to `head.html`

l.38: `<link href="{{#site}}{{root}}{{/site}}extra.css" rel="stylesheet">` -> Otherwise the changes in `extra.css` will not be applied to the theme but will completely inherit from the bootstrap theme.

