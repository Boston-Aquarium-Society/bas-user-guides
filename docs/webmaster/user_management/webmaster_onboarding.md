The webmaster (or someone else who should have full admin access to the club's
web presence) will need access to a variety of accounts.


## Prerequisites

If the new webmaster does not already have accounts for the following sites,
they must create them first

1. Google (*i.e.* you will need an `@gmail.com` account)
1. DigitalOcean (It is best to select "Sign up with Google" so your account
   is already associated with your Gmail account)
1. Github account

## Granting access

The following can only be done by the previous webmaster:

1. Once logged into 1Password, navigate to [my.1password.com/people](https://my.1password.com/people).
   * Invite the new webmaster. They will need to accept the invitation before
     they are able to view the passwords.
   * Once they have activated their account, edit their membership so that they are a
     manager of the `Owners` and `Administrators` groups.
1. In Digital Ocean, log into the BAS project, open the "Settings" tab, and then
   `Invite Members`.
1. In Github, go to the [user page][bas-github], and invite them as a user.
1. Follow the [Site Staff instructions](/webmaster/user_management/site_staff).
   They should get `Administrator` permissions.
1. Follow the [Calendar instructions](/webmaster/user_management/calendar).

## Digital Ocean Access

In order to access our VM, the user will need a SSH key. If the new webmaster
needs instructions on how to generate a SSH key, they can be found
[here][ssh-key-instructions].

They should send you their SSH public key ([instructions][ssh-pub-key]). That
public key should be added to the `authorized_keys` file of our DO droplet.
([instructions][add-pub-key-to-droplet]).

## Google Analytics Access

To view site usage statistics, you will need access to [Google Analytics][google-analytics].

Follow [these instructions][google-analytics-add-user] for adding a new user.

[bas-github]: https://github.com/orgs/Boston-Aquarium-Society/people
[ssh-key-instructions]: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
[ssh-pub-key]: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account
[add-pub-key-to-droplet]: https://docs.digitalocean.com/products/droplets/how-to/add-ssh-keys/to-existing-droplet/#manually
[google-analytics]: https://analytics.google.com/analytics/web
[google-analytics-add-user]: https://support.google.com/analytics/answer/1009702?hl=en#Add&zippy=%2Cin-this-article
