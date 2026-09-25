# Mod catalog

Served to the PPG Safe Loader. Every entry here is signed with the reviewer's private key,
which is not in this repository and never will be.

Write access to this repository grants **no** ability to publish a mod. The loader verifies the
signature over `manifest.json` before it trusts a single byte, and each download's SHA-256 is
inside that signature, so a swapped file is refused.

Do not edit `manifest.json` by hand — any edit invalidates the signature and the loader will
reject the whole catalog.
