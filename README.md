# Bootstrap Default
Installation profile with bootstrap codebase

## Reuse YML files
Remove all of the UUIDs and default_config_hash from your config files so that they don't conflict with those of new sites. This can be done quite easily on the command line like so all on one line:

find /path/to/PROFILE_NAME/config/install/ -type f -exec sed -i -e '/^uuid: /d' {} \;

find /path/to/PROFILE_NAME/config/install/ -type f -exec sed -i -e '/_core:/,+1d' {} \;
