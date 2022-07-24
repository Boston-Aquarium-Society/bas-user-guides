Static content describes things like forms or files that visitors will download
from the website. Examples of static content include [membership forms][membership-form]
and a [PDF containing the history of the BAS][history-of-bas].

Unfortunately, the Ghost blogging platform doesn't provide tools for uploading
static content through the website itself. Instead, you must upload content
directly to the server running the site. As such, it's generally easiest to ask
the webmaster to do this for you.

## Upload via SCP

!!! important

    This requires SSH access to the VM running the BAS site.
    Instructions for this can be found [here](../../webmaster/user_management/webmaster_onboarding.md#granting-access).

To upload the file `file-to-upload.pdf`, you would first `scp` it into the VM
(make sure to provide the correct path to the file):

```terminal
scp /path/to/file-to-upload.pdf root@{{ site.base_url }}:/var/www/ghost/static/
```

Once files have been uploaded, they are immediately available at the URL `https://{{ site.base_url }}/static/<NAME-OF_FILE>`.
Therefore, the example file would be accessable at `https://{{ site.base_url }}/static/file-to-upload.pdf`.

[history-of-bas]: https://{{ site.base_url }}/static/history_of_the_boston_aquarium_society.pdf
[membership-form]: https://{{ site.base_url }}/static/BASapplication.pdf
