# Keeping these guides current

These guides are only useful if they match how things actually work today.
If they drift, the next person to pick up a role is stuck guessing.

## The rule

Whenever a role or a procedure changes, update the guide in the same week.
That includes things like:

* A new officer, webmaster or content maintainer takes over (update who
  should have what access, not people's names or contact details).
* We start or stop using a service (hosting, Cloudflare, Mailgun, Google,
  1Password, etc.).
* We fix something in a new way, like blocking a spam bot or recovering
  from an outage. Write the runbook while it's fresh.
* A step in an existing guide turns out to be wrong or out of date.

If you don't have time to write it up properly, open a GitHub issue that
says what changed so it isn't lost.

## What not to put in here

These guides are published on the public docs site. Don't commit:

* Passwords, API keys, tokens or other secrets. Point to 1Password instead.
* Member personal details (emails, phone numbers, addresses), including
  member exports or backups.

## How to make a change

1. Create a branch and edit the Markdown under `docs/`.
2. If you add a page, add it to the `nav` in `mkdocs.yml`.
3. Check it builds: `mkdocs build --strict` (see the README for setup).
4. Open a pull request. Once it merges to `main`, the docs site redeploys
   on its own.

## Regular review

Each time you do the quarterly site maintenance, skim the Webmaster pages
and fix anything that no longer matches what you just did. Each page shows
when it was last updated at the bottom, which makes stale pages easy to spot.
