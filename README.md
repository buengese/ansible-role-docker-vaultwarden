ansible-role-vaultwarden
===================
Quick and dirty ansible role to setup [Vaultwarden](https://github.com/dani-garcia/vaultwarden) via docker compose. This role depends on docker and docker-compose<2.0 as well as the python docker-sdk.


Role Variables
--------------

The following variables determine the install and update behaviour of this role.

* `vaultwarden_domain`: The domain Vaultwarden will be reachable on.
* `vaultwarden_admin_token`: The Vaultwarden admin token.
* `vaultwarden_compose_dir`: The directory where docker compose files will be stored.
* `vaultwarden_volume_dir`: The docker volume dir for Vaultwarden.


Supported OS
------------
- Ubuntu
- Debian
- Fedora
- ArchLinux


License
-------

MIT
