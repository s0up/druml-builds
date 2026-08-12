# DruML Builds

Public distribution repository for [DruML](https://druml.ai) — an AI-driven USB MIDI instrument training system.

This repository serves two purposes:

1. **Fleet firmware** — the signed firmware builds that DruML devices in the field update to.
2. **CAD library** — the evolving set of printable and laser-cuttable parts, published so owners can make their own hardware.

Nothing here is the DruML application source; this is the public delivery channel for the things that need to reach hardware and makers.

---

## Fleet firmware

Every fleet release is published under [Releases](https://github.com/s0up/druml-builds/releases). Each release contains the signed firmware image for the current generation of DruML hardware, along with release notes describing what changed in detection, training behavior, and playability.

- **Latest stable** — the release marked `Latest`. This is what devices receive by default.
- **Pre-releases** — early builds published for testing ahead of a general rollout.

Devices update themselves; there is normally no reason to download an image by hand. Release notes are the best place to see what a given version changed.

Versions follow `vMAJOR.MINOR.PATCH.BUILD`, where the build number is a monotonically increasing counter across the whole fleet history.

---

## CAD library

The [`3d_models/`](3d_models) directory holds the current revision of DruML's mechanical parts. These files are updated as the hardware evolves, so treat the newest revision in the directory as the source of truth.

### 3D printed parts (`.3mf`)

| File | Description |
| --- | --- |
| `basket_10in_unibody_minimal.3mf` | 10" unibody basket, minimal profile |
| `basket_12in_r4.3mf` | 12" basket, revision 4 |
| `basket_13in_r4.3mf` | 13" basket, revision 4 |
| `basket_14in_r4.3mf` | 14" basket, revision 4 |
| `basket_16in_r4.3mf` | 16" basket, revision 4 |
| `piezo_standoff_18mm.3mf` | 18 mm piezo standoff |

`.3mf` files carry their own geometry and can be opened directly in most slicers (Bambu Studio, PrusaSlicer, Orca, Cura).

### Laser cut parts (`.dxf`)

| File | Description |
| --- | --- |
| `acrylic_hub_rev0.6.dxf` | Full-size acrylic hub, revision 0.6 |
| `acrylic_hub_mini_rev0.1.dxf` | Mini acrylic hub, revision 0.1 |

`.dxf` files are 1:1 and intended for acrylic. Confirm your machine imports them at true scale before cutting, and check kerf compensation against a test piece.

### Printing notes

Parts are designed to be printed without supports in their supplied orientation. Baskets are sized per drum diameter — match the file to your drum, not to your printer bed.

---

## Contributing and issues

Revisions here track the hardware, so files change over time. If you print or cut a part and find a fit problem, open an issue with the file name, revision, and what you measured — that feedback is what drives the next revision.

## Links

- **Website** — [druml.ai](https://druml.ai)
- **Releases** — [github.com/s0up/druml-builds/releases](https://github.com/s0up/druml-builds/releases)
