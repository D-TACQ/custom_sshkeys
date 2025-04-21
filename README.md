custom_sshkeys:

SITE key customization. Enables ssh passwordless login using key exchange
Install your own "authorized keys" on every UUT at your site

* Update authorized_keys
* in make.release, set SITE to something more meaningful for your site
* sudo ./make.release
* deploy release/15-SITE_sshkeys.YYMMDD.gz to /mnt/packages on every UUT on your site.
* nb: you'll have to re-activate after every firmware upgrade, simplest approach is to keep a copy in /mnt/local and copy across after update.

* Possibility for other simple SITE customisation, eg custom network settings.


