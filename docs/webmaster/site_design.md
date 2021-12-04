The source code for the {{ site.url }} theme (*i.e.* how the site is themed and
styled) is found [here][ghost-theme]. Most site updates can be done from the web
UI. Updating the theme is only necessary to customize the site HTML.

To learn more about how themes work for Ghost (the platform our site is based
on), you can read the docs [here][ghost-theme-docs]. Our theme's landing page
contains instructions on how to make changes and test them locally.

Continuous deployment is configured on the theme so that changes are automatically
applied to {{ site.url }} when pull requests are merged to the default branch.

[ghost-theme]: {{ site.theme_source }}
[ghost-theme-docs]: https://ghost.org/docs/themes/structure/
