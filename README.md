ansible-role-vaultwarden
===================
Quick and dirty ansible role to setup [Vaultwarden](https://github.com/dani-garcia/vaultwarden) to run as a Docker container wrapped in a systemd service.


Role Variables
--------------
### Core Variables
Key variables that are required for the role’s operation include:

- `vaultwarden_hostname`: Hostname for the Vaultwarden instance. i.e. `vaultwarden.example.com`

Addionally these variables are not required but commonly used:

- `vaultwarden_config_admin_token`: Token for accessing the Vaultwarden admin interface. If unset a token will be automatically generated and displayed at the end of role execution.
- `vaultwarden_container_http_bind_port`: Controls whether (and how) the container exposes its HTTP port.
- `vaultwarden_database_type`: Controls which database type is used. Possible values: `sqlite`, `postgres`

Check [defaults/main.yml](defaults/main.yml) for the full list of supported options.

Supported OS
------------
- Ubuntu
- Debian
- Fedora
- ArchLinux
- pretty much everything that has docker

License
-------

GPL-3.0-or-later
