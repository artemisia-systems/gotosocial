# Gotosocial
If you want to know about gotosocial itself, go check [the actual repo](https://github.com/superseriousbusiness/gotosocial).
All I'm doing is making my little allowlist patch available.

# Changes
So far the only change from stock gotosocial is that this fork enforces allowlist federation: traffic from remote instances not explicitly listed under AllowedDomains in the config file is dropped when we would otherwise check their keys.

# This repo
The main branch directly tracks upstream gotosocial and rebases all patches directly on top every time. In other words, my commits will always show up as the most recent keeping this fork easy to compare to upstream.

Various branches are provided as separate "release" tracks: experimental also tracks upstream directly and is rebased off of main whenever new commits don't give me a bad feeling; unstable floats somewhere between actual gotosocial releases if I think there are features worth fastforwarding to (like search); stable is pinned to the most recent gotosocial release with my changes applied.
Depending on upstream, this means stable may not be a direct ancestor commit of unstable/experimental/main such as when v0.9.1 backported some but not all of features present on my unstable track at the time (namely lists were ommitted).
As a result, stable may counter-intuitively be a less stable release track than unstable which at least is guaranteed to be advanced along to a version that at some point represented the head of the experimental track.

