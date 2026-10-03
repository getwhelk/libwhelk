# libwhelk

The stable C ABI library for [Whelk](https://getwhelk.com), and the Apache-2.0
language bindings over it.

Whelk is the platform for private AI. `libwhelk` exposes a small, stable C ABI
over Whelk's portable core, for callers that are not Swift or Kotlin. The
library ships as a signed binary and the committed C header beside it. Whelk is
open core, and the core this library wraps is licensed Apache-2.0. Its source is
not in this repository.

## What ships here

- **Signed libraries and the C header**, as release assets. The macOS library
  is a universal (arm64 + x86_64) dylib, Developer ID signed and notarized. The
  Linux library is an x86_64 shared and static library. Each release lists the
  SHA-256 of every file.
- **The Apache-2.0 bindings** (Python, JavaScript, Node) as their own package
  release. Those are the thin glue over the C ABI; they hold no proprietary
  logic.

See the [latest release](https://github.com/getwhelk/libwhelk/releases/latest).
