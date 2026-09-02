# Curacast — Unraid Community Applications templates

Container templates for [Curacast](https://curacast.tv), which turns a Plex,
Jellyfin or Emby library into 24/7 live TV channels with a real programme guide.

This repository exists so Unraid's **Community Applications** can read the
templates. It holds no source code — Curacast itself is closed source.

| Template | Use it when |
| --- | --- |
| `curacast.xml` | Standard install. Software encoding, or Intel/AMD via `/dev/dri`. |
| `curacast-nvidia.xml` | You want NVENC hardware transcoding on an Nvidia GPU. |

## Installing

You do not need this repository. In Unraid, open the **Apps** tab, search for
**Curacast**, and click Install.

## What the templates configure

- **WebUI and HDHomeRun tuner** on port `8000`
- **Appdata** at `/home/curacast/app/.curacast` — channels, settings and your
  licence live here, so map it to real storage
- Image: [`curacast/curacast`](https://hub.docker.com/r/curacast/curacast),
  published for `linux/amd64` and `linux/arm64`

## Support

Email <support@inertiatechgroup.com>, or see
[curacast.tv/support](https://curacast.tv/support).

Curacast is a product of Inertia Tech Group LLC.
