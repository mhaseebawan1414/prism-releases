# PRISM App releases

Signed release artifacts for PRISM App. Source lives in the private
`mhaseebawan1414/prism` repo; this repo holds only built, signed artifacts so the
in-app updater (`Prism.Updater`) never needs a credential that can read private source.

Each release's `current.json` is a manifest (product version + per-file SHA-256 hashes),
signed RSA-3072/PSS/SHA-256. Verify with the public key embedded in
`Prism.Updater/TrustedSigningKey.cs` in the source repo.
