# TodoitBot Windows browser engine (mirror)

This public repository redistributes an unmodified copy of the Windows
`agent-browser` build that TodoitBot downloads at install time. Hosting the
file here means a TodoitBot install does not have to fetch it from an upstream
project it no longer depends on.

The executable is bit-for-bit identical to the reviewed vendor build published
as [browser-engine-v0.36.0-omb.1](https://github.com/milind-soni/OpenMausBot/releases/tag/browser-engine-v0.36.0-omb.1)
by the OpenMausBot project. TodoitBot is a fork of OpenMausBot and keeps the
Apache-2.0 attribution that license requires.

## Asset

| Field | Value |
| --- | --- |
| File | `agent-browser-win32-x64-0.36.0-omb.1.exe` |
| Version | `0.36.0-omb.1` |
| SHA-256 | `33bee834f6a6072ec8688b0914726e0262874d758f69f27e8baf7eaac6b5ed15` |
| Size | 13,806,080 bytes |
| Download | https://github.com/SIRAJcrypto11/todoitbot-browser-engine/releases/download/browser-engine-v0.36.0-omb.1/agent-browser-win32-x64-0.36.0-omb.1.exe |

Do not replace this file with a rebuilt binary under the same name or tag
unless the digest above is updated in TodoitBot (`server/browser-engine-release.ts`)
after a reviewed native end-to-end run.

## Provenance and license

- The vendor build starts from [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) v0.36.0 (Apache License 2.0) and carries only the Windows handle-inheritance fix from [PR 1781](https://github.com/vercel-labs/agent-browser/pull/1781). The patch, provenance record, and upstream license texts are in `notices/`.
- `LICENSE` in this repository is the Apache-2.0 text shipped with that agent-browser release.
- OpenMausBot, Copyright 2026 Milind Soni and OpenMausBot contributors, licensed under Apache-2.0.
- TodoitBot / this mirror: PT SNISHOP NETWORK INDONESIA redistributes the same file unchanged so TodoitBot clients can download it without authentication.
- The names OpenMausBot, MausBot, Vercel, and agent-browser remain their owners' marks. This mirror does not imply endorsement.

This is not a source repository for the engine and is not the TodoitBot application. The application lives at the SNISHOP TodoitBot project.
