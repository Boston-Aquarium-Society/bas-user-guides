Club members will need to be site staff members in order to create pages,
post articles, etc.

Whenever possible, please give users the lowest possible permission level to
keep our site secure. Information about the different permission levels can be
found [here][staff-docs].

In general, the only people who should be "Administrators" are the webmaster(s)
and the club president (or designee) as a backup. Everyone else should have a
lower permission level.

The "Contributor" level is best, as it allows users to create new posts, but
requires that the webmaster review and approve the article before it is posted
live on the site.

## How to add a new member

1. Navigate to the [staff management page][staff-management]
1. Click `Invite people` and enter the user's email address.
1. Select the appropriate permission level (ideally contributor) and send the
   invitation
1. Let the user know that they have been sent an invitation link via email that
   they will need to accept before they get access to the site.

User permissions can be upgraded, downgraded, or suspended by an admin once
the user has accepted the invitation and joined.

## When officers change

Site access follows the role, not the person. When a new president or
webmaster takes office (after the board vote, not before):

1. Give the incoming president (or their designee) `Administrator` access.
1. Downgrade the outgoing president to the lowest level they still need, or
   suspend them if they no longer need access.
1. Check the other places the president or webmaster has access: the club
   Google calendar, Google Analytics, 1Password, DigitalOcean, Cloudflare and
   Github. For a new webmaster, follow
   [New Webmaster Onboarding](webmaster_onboarding.md).
1. Update these guides if anything about the roles changed.

[staff-docs]: https://ghost.org/docs/staff/
[staff-management]: https://{{ site.base_url }}/ghost/settings/staff/
