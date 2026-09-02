# Curacast — Unraid Community Applications templates

Container templates for [Curacast](https://curacast.tv), which turns a Plex,
Jellyfin or Emby library into 24/7 live TV channels with a real programme guide.

This repository exists so Unraid's **Community Applications** can read the
template. It holds no source code — Curacast itself is closed source.

`templates/curacast.xml` is the container template. Intel and AMD GPUs can be
passed through for hardware transcoding by adding `/dev/dri`. An NVIDIA variant
is not published yet — it needs an image built against the NVIDIA runtime.

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

## Licence

[Apache License 2.0](LICENSE), covering **these templates and their
documentation only**. Curacast itself is proprietary software under a separate
commercial licence — see [curacast.tv](https://curacast.tv) and [NOTICE](NOTICE).

Apache 2.0 was chosen over MIT for its explicit trademark clause: the licence
grants no right to use the Curacast name.

Curacast is a product of Inertia Tech Group LLC.
