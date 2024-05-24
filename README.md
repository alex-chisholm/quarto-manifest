# Individual quarto file

If there are multiple individual quarto docs, use `appPrimaryDoc` to specify the intended doc.

```
library(rsconnect)
writeManifest(appPrimaryDoc='report2.qmd')
```

manifest.json

```

{
  "version": 1,
  "locale": "en_US",
  "platform": "4.3.2",
  "metadata": {
    "appmode": "quarto-static",
    "primary_rmd": "report2.qmd",
    "primary_html": null,
    "content_category": null,
    "has_parameters": false
  },
  "quarto": {
    "version": "1.4.549",
    "engines": ["knitr"]
  },
  
  .....
  
  
  

```


# Sites

If the output is a complex quarto type (site, blog, book, etc...). 

```
writeManifest(appDir='book', appPrimaryDoc = 'index.html', contentCategory='site')
```

manifest.json:

```

{
  "version": 1,
  "locale": "en_US",
  "platform": "4.3.2",
  "metadata": {
    "appmode": "quarto-static",
    "primary_rmd": "index.html",
    "primary_html": null,
    "content_category": "site",
    "has_parameters": false
  },
  "quarto": {
    "version": "1.4.549",
    "engines": ["markdown"]
  },
  
  .......

```
