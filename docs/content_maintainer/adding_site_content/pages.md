"Pages" on the BAS website contain information about the club and don't change frequently.
They include the [about page][about-page] or the [auctions policy][auctions-page].
They almost always appear in the primary navigation bar at the top of every page, or in the footer navigation.

## Adding a new page

* Start on the [new page editor][new-page]
* Open the page settings (by clicking on the rectangular icon in the upper right-hand corner of the page)
* In the "Page URL" section, give the page a short, easy to spell URL.
* Set the post author to be "BAS Webmaster" (and deselect your own name).
* Using the text editor, give the page a title, then type the body of the page.
    * You can read more about how to use the text editor to create a good-looking page [here][ghost-editor-faq].
* **Important**: After finishing, make sure to publish the article! (Click "Publish")

!!! question
    * Have you remembered to publish the post using the publish button?

## Adding a page to the navigation menu

After a page has been created and published, it can be added to the navigation menu.
First, start by going to the [navigation settings][navigation-menu-edit].

The "Primary navigation" is the list of links that appear at the top of each page.
Only the first 5 links appear! All additional links are collapsed into a `...` section.

The "Secondary navigation" is the list of links that appears at the bottom of each page.
There is not a limit to how many links appear here (except that there should not
be so many links as to make it look cluttered).

When adding a new page to the navigation, give it a short, clear name and then
include the page URL. (You previously set the URL when creating the page).
Then, click the green `+` button next to the new entry.
Finally, click the "Save" button at the top of the page.

!!! important
    After adding a new link, go to the home page and click the link to make sure
    it works. It's not good to have broken links on the site!

[about-page]: https://{{ site.base_url }}/about
[auctions-page]: https://{{ site.base_url }}/auctions
[bas-homepage]: https://{{ site.base_url }}
[ghost-editor-faq]: https://ghost.org/help/using-the-editor
[navigation-menu-edit]: https://{{ site.base_url }}/ghost/#/settings/navigation
[new-page]: https://{{ site.base_url }}/ghost/#/editor/page
