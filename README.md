# ba-kets.github.io

Sovereign identity host for **asif** — Nostr NIP-05 + Lightning-address.

## What this serves

- **NIP-05**: `asif@ba-kets.github.io` — verified Nostr identity
- **LNURL-pay**: `asif@ba-kets.github.io` — Lightning-address (pending channel funding)
- **/index.html**: public landing page

## Cryptographic identity

```
npub: npub18l8urveppv43e2wam6htkn08ayrm0nurwwxjsevnfqfjwsfehpeqga8l97
hex:  3fcfc1b3210b2b1ca9dddeaebb4de7e907b7cf83738d2865934813274139b872
```

## How clients verify

When a Nostr-client checks `asif@ba-kets.github.io`:
1. GET `https://ba-kets.github.io/.well-known/nostr.json?name=asif`
2. Reads `names.asif` from response
3. Matches against profile's pubkey
4. ✓ Verified badge shown

## Stack behind this identity

Bitcoin Core full node · LND Lightning · Fulcrum indexer · Tor + I2P + CJDNS · Self-hosted Mempool · Custom Nostr relay (strfry)

## License

MIT — fork freely.
