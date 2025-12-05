# obs-ls-headless plugin backup

JSON-RPC plugin that backs up a local notes directory to remote storage (S3/OSS, etc.), driven by Host events. Intended as a minimally invasive extension for [obs-ls-headless](https://github.com/narcotics726/obs-ls-headless).

Current status: skeleton only; protocol and backup logic not implemented yet.

## Planned features
- JSON-RPC 2.0 over stdin/stdout using Content-Length framing.
- Plugin-initiated handshake declaring subscribed events (SyncStarted/SyncCompleted/SyncFailed).
- Incremental/full backups with a bias toward data preservation; remote targets via adapter pattern (S3/OSS first).
- Planned snapshot rotation and lightweight log/status notifications.

## License
MIT
