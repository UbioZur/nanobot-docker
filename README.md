<p align="center">
  <img src="https://raw.githubusercontent.com/HKUDS/nanobot/main/images/readme-cover-light.svg" alt="nanobot" width="160">
</p>

<h1 align="center">Nanobot Docker</h1>

<p align="center">
  My continuously built, signed Docker image of
  <a href="https://github.com/HKUDS/nanobot">HKUDS/nanobot</a>.
</p>

<p align="center">
  <a href="https://github.com/UbioZur/nanobot-docker/actions/workflows/build.yml">
    <img src="https://github.com/UbioZur/nanobot-docker/actions/workflows/build.yml/badge.svg" alt="Build">
  </a>
  <a href="https://github.com/UbioZur/nanobot-docker/pkgs/container/nanobot-docker">
    <img src="https://img.shields.io/badge/ghcr.io-image-blue?logo=docker" alt="GHCR">
  </a>
  <img src="https://img.shields.io/docker/image-size/ubiozur/nanobot-docker/latest?sort=date&logo=docker" alt="Image size">
  <img src="https://img.shields.io/github/license/UbioZur/nanobot-docker" alt="License">
</p>

---

## About

This repository provides a Docker image for
[**nanobot**](https://github.com/HKUDS/nanobot), an ultra-lightweight,
self-hosted personal AI agent framework.

The image is built automatically from the upstream nanobot repository.

### Image lifecycle

- Builds from official upstream nanobot releases.
- Automatically checks for new upstream tags every week.
- Publishes versioned images such as `v0.3.0`.
- Maintains the `latest` tag for the newest upstream release.
- Dockerfile and `docker-compose.yml` changes are detected and reported through a GitHub issue.
- Images are signed with [Cosign](https://docs.sigstore.dev/cosign/).
- No additional nanobot channels are preinstalled by default.

Upstream project:

**[HKUDS/nanobot](https://github.com/HKUDS/nanobot)**

---

## Docker image

Images are published to GitHub Container Registry:

```text
ghcr.io/ubiozur/nanobot-docker
```

Pull the latest image:

```bash
docker pull ghcr.io/ubiozur/nanobot-docker:latest
```

Or pull a specific upstream release:
```bash
docker pull ghcr.io/ubiozur/nanobot-docker:v0.3.0
```