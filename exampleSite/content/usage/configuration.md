## Site configuration

{{< tabs "site-config" >}}
{{< tab "TOML" >}}

```Toml
[params]
  # (Optional, default 6) Set how many table of contents levels to be showed on page.
  # Use false to hide ToC, note that 0 will default to 6 (https://gohugo.io/functions/default/)
  # You can also specify this parameter per page in front matter.
  geekdocToC = 3

  # (Optional, default static/brand.svg) Set the path to a logo for the Geekdoc
  # relative to your 'static/' folder.
  geekdocLogo = logo.png

  # (Optional, default false) Render menu from data file im 'data/menu/main.yaml'.
  geekdocMenuBundle = true

  # (Optional, default true) Show page navigation links at the bottom of each
  # docs page (bundle menu only).
  geekdocNextPrev = false

  # (Optional, default true) Show a breadcrumb navigation bar at the top of each docs page.
  # You can also specify this parameter per page in front matter.
  geekdocBreadcrumb = false

  # (Optional, default none) Set source repository location
  # Used for 'Edit this page' links
  # You can also specify this parameter per page in front matter.
  geekdocRepo = 'https://github.com/xoxys/hugo'

  # (Optional, default none) Enable "Edit this page" links. Requires 'GeekdocRepo' param
  # and path must point to 'content' directory of repo.
  # You can also specify this parameter per page in front matter.
  geekdocEditPath = 'edit/master/exampleSite/content'

  # (Optional, default 'Jan 2, 2006') Configure the date format used on the pages in blog posts.
  geekdocDateFormat = "Jan 2, 2006"

  # (Optional, default true) Enables search function with flexsearch.
  # Index is built on the fly and might slowdown your website.
  geekdocSearch = false
```

{{< /tab >}}
{{< tab "YAML" >}}

```Yaml
params:
  # (Optional, default 6) Set how many table of contents levels to be showed on page.
  # Use false to hide ToC, note that 0 will default to 6 (https://gohugo.io/functions/default/)
  # You can also specify this parameter per page in front matter.
  geekdocToC: 3

  # (Optional, default static/brand.svg) Set the path to a logo for the Geekdoc
  # relative to your 'static/' folder.
  geekdocLogo: logo.png

  # (Optional, default false) Render menu from data file im 'data/menu/main.yaml'.
  # See also https://geekdocs.de/usage/menus/#bundle-menu
  geekdocMenuBundle: true

  # (Optional, default true) Show page navigation links at the bottom of each
  # docs page (bundle menu only).
  geekdocNextPrev: false

  # (Optional, default true) Show a breadcrumb navigation bar at the top of each docs page.
  # You can also specify this parameter per page in front matter.
  geekdocBreadcrumb: false

  # (Optional, default none) Set source repository location
  # Used for 'Edit this page' links
  # You can also specify this parameter per page in front matter.
  geekdocRepo: https://github.com/xoxys/hugo-geekdoc

  # (Optional, default none) Enable "Edit this page" links. Requires 'GeekdocRepo' param
  # and path must point to 'content' directory of repo.
  # You can also specify this parameter per page in front matter.
  geekdocEditPath: edit/master/exampleSite/content

  # (Optional, default 'Jan 2, 2006') Configure the date format used on the pages in blog posts.
  geekdocDateFormat: "Jan 2, 2006"

  # (Optional, default true) Enables search function with flexsearch.
  # Index is built on the fly and might slowdown your website.
  geekdocSearch: false
```

{{< /tab >}}
{{< /tabs >}}

## Page configuration

{{< tabs "page-config" >}}
{{< tab "TOML" >}}

```Toml
# Set type to 'posts' if you want to render page as blogpost
type = 'posts'

# Set page weight to re-arrange items in file-tree menu
weight = 10

# Set how many table of contents levels to be showed on page.
geekdocToC = 3

# Show a breadcrumb navigation bar at the top of each docs page.
geekdocBreadcrumb = false

# Set source repository location
geekdocRepo = 'https://github.com/xoxys/hugo-geekdoc'

# Enable "Edit this page" links. Requires 'GeekdocRepo' param and path must point
# to 'content' directory of repo.
geekdocEditPath = 'edit/master/exampleSite/content'

# Used for 'Edit this page' link, set to '.File.Path' by default.
# Can be overwritten by a path relative to 'geekdocEditPath'
geekdocFilePath =

# Set to mark page as flat section (file-tree menu only)
geekdocFlatSection = true

# Set true to hide page or section from side menu (file-tree menu only)
geekdocHidden = true
```

{{< /tab >}}
{{< tab "YAML" >}}

```Yaml
# Set type to 'posts' if you want to render page as blogpost
type: 'posts'

# Set page weight to re-arrange items in file-tree menu
weight: 10

# Set how many table of contents levels to be showed on page.
geekdocToC: 3

# Show a breadcrumb navigation bar at the top of each docs page.
geekdocBreadcrumb: false

# Set source repository location
geekdocRepo: https://github.com/xoxys/hugo-geekdoc

# Enable "Edit this page" links. Requires 'GeekdocRepo' param and path must point
# to 'content' directory of repo.
geekdocEditPath: edit/master/exampleSite/content

# Used for 'Edit this page' link, set to '.File.Path' by default.
# Can be overwritten by a path relative to 'geekdocEditPath'
geekdocFilePath:

# Set to mark page as flat section (file-tree menu only)
geekdocFlatSection: true

# Set true to hide page or section from side menu (file-tree menu only)
geekdocHidden: true
```

{{< /tab >}}
{{< /tabs >}}