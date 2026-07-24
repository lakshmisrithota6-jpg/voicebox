# voicebox

This workspace is prepared for installing [jamiepine/voicebox](https://github.com/jamiepine/voicebox), the open-source local AI voice studio.

## Install status

The target runtime for this container is Linux (`x86_64`). Voicebox currently documents Docker as the supported Linux install path, while pre-built Linux desktop binaries are not yet available.

The source install requires access to GitHub plus the project prerequisites:

- Bun
- Rust
- Python 3.11+
- Tauri system prerequisites
- `just`

## Standard source install

```bash
git clone https://github.com/jamiepine/voicebox.git
cd voicebox
just setup
just dev
```

## Docker install

```bash
git clone https://github.com/jamiepine/voicebox.git
cd voicebox
docker compose up
```

## Environment note

I attempted to fetch the upstream repository directly in this environment, but outbound access to GitHub tarballs and `git clone` was blocked by HTTP 403 responses. Once GitHub access is available, use one of the install paths above.
