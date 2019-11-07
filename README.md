
# mlr3pkgdowntemplate

pkgdown template files for all mlr* related packages.

# Changes to original pkgdown templates

All custom changes live in `inst/pkgdown/css/extra.css`

## Changes to `pkgdown.css`

l.125:   `height: 16px;` -> otherwise the orcid icon is oversized

## Changes to `head.html`

l.38: `<link href="{{#site}}{{root}}{{/site}}extra.css" rel="stylesheet">` -> Otherwise the changes in `extra.css` will not be applied to the theme but will completely inherit from the bootstrap theme.

l.23: Custom bootstrap theme. See https://github.com/r-lib/pkgdown/issues/1176

  ```js
  {{^bootswatch}}<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">{{/bootswatch}}
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
  ```
