# VAULT — playable ad

A playable ad that ships as one small HTML file, with everything drawn and synthesised at runtime.

**[Play it](https://akultange.github.io/vault-playable/)** · **[Recording](https://akultange.github.io/vault-playable/vault_recording.mp4)**

## Highlights

- **Single self-contained HTML, ~25 KB.** One file per build, no bundler, no dependencies.
- **Zero binary assets.** All art is drawn in code, and all sound is procedural WebAudio.
- **~300-particle physics** with spatial hashing, running at 60 fps.
- **Two levels.** A tutorial, then an order-trap level with a fail state.
- **Runtime CTA network detection.** One handler picks the right exit call, checked in this order: `FbPlayableAd` → `ExitApi` → `dapi` → `mraid`.

## Builds

| Build | File | Target |
| --- | --- | --- |
| Meta | [vault_meta.html](builds/vault_meta.html) | Single-file playable |
| Google Ads | [vault_google_ads.zip](builds/vault_google_ads.zip) | ZIP with `ExitApi` |
| MRAID | [vault_mraid.html](builds/vault_mraid.html) | Unity, AppLovin, Mintegral, Vungle (ironSource via `dapi`) |

The `index.html` at the repo root is the browser preview build that the "Play it" link serves.

Concept & code: Luka Skhiladze
