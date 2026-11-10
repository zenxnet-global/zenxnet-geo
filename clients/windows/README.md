# ZENXNET Windows GEO snapshot

This directory is the Windows compatibility profile. It is separate from the RU/PRIVATE-only databases at the repository root and is not replaced by the root build-geo workflow.

The initial snapshot preserves the exact databases shipped with ZENXNET Windows on 2026-11-09. Moving the download source here does not change any IP ranges, domain entries, rule ordering, DNS settings or routing policy.

| Database | Categories required by current panel templates |
| --- | --- |
| geoip.dat | DIRECT, PRIVATE |
| geosite.dat | CATEGORY-RU, GOOGLE-PLAY, PRIVATE, TWITCH |

The IP database also includes WHITELIST. DIRECT is a curated routing list; it must not be replaced with or aliased to the general RU country category.

Windows pins the complete Git commit and SHA-256 of both files in its own `geo.lock.json`. Updating these files is a separate reviewed data change: compare normalized IP ranges and domain entries, verify all referenced categories with the pinned Xray version, and update the Windows lock. Do not switch Windows to root `geoip.dat` or to a moving branch URL.

See [PROVENANCE.md](PROVENANCE.md), [SHA256SUMS](SHA256SUMS) and [geosite-LICENSE.txt](geosite-LICENSE.txt) for the sources, exact hashes and retained license.
