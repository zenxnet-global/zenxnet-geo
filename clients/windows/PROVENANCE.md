# Snapshot provenance

Snapshot prepared by Codex for ZENXNET on 2026-11-10. The binaries are copied without modification from the verified ZENXNET Windows installer resources; they are not newly generated lists.

- `geoip.dat`: original snapshot https://github.com/hydraponique/roscomvpn-geoip/releases/tag/202611041049 ; SHA-256 `9842938ee7f9309591f6534edd2bf233957474848bf78fd9a1dcc6da7e0323f4`.
- `geosite.dat`: original snapshot https://github.com/hydraponique/roscomvpn-geosite/releases/tag/202610120948 ; SHA-256 `6fadc9298116c5523b1e3cfa46c6c5fed5a218b9b6365be831e358f4823ea464`. This file already matches the database at repository root commit `97d40c00f797df9db930eccf3de9ee9dc463b7f5`.

The geosite source distributes its database under the MIT license, copyright V2Ray 2018–2019; the full notice is retained alongside the data. The geoip upstream README lists GeoLite2, IPinfo, DB-IP and Re:filter as its source data. This snapshot does not assert a new license or independent authorship over those underlying databases. Preserve their provenance and applicable terms when updating or redistributing the data.

The purpose of this profile is an independently pinned ZENXNET distribution path with unchanged Windows routing behavior. Updating or replacing the underlying datasets requires separate compatibility review.
