# GoToSocial <!-- omit in toc -->

If you want to know about gotosocial itself, go check [the actual repo](https://github.com/superseriousbusiness/gotosocial).
All I'm doing is making my little allowlist patch available.

This just adds a new key to the config, "allowed-domains" which should be a list of strings corresponding to instances on the allowlist.
Personally, I do all the actual configuration through environment variables so I just use my allowlist.yml as the sole config file.
