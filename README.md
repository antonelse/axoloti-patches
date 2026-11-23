# axoloti-patches

Patches for the [Axoloti](https://ksoloti.github.io/2-background.html) DSP environment, by Johannes Taelman.

**Tested hardware:** Axoloti Core v1.2. Ksoloti, the successor platform, is not tested. Objects are not always compatible between the two, so check before porting.

## Patches

| Patch | Folder | Latest | Description |
|-------|--------|--------|-------------|
| AnDrone | [`androne/`](./androne) | v2.1.0 | Six-oscillator drone synth, inspired by Guilherme Martins' Drone Engine. Scale quantisation, 3x3 matrix mixer, piezo line input. |
| AxoGlitch | [`axoglitch/`](./axoglitch) | v5 | Glitch processor. Guide in preparation. |

## Controllers

- **AnDrone** is controlled from an M-Audio Evolution UC33e. The mapping, presets and CC table are in [MIDI-mappings-ae](https://github.com/antonelse/uc33e-mappings) (presets P23–P25).
- **AxoGlitch** is controlled from a Korg nanoPAD. Its mapping is documented in `axoglitch/`.

## Repository layout

```
axoloti-patches/
├── androne/
│   ├── GUIDE.md        overview, patch analysis, mixer, scale/key
│   ├── CHANGELOG.md
│   ├── patch/          released .axp files
│   ├── extra/          original Guilherme Martins patch and mapping images
│   └── imgs/
└── axoglitch/
    └── ae_AxoGlitch_v*.axp
```

## Notes

Patch files are Axoloti patcher projects (`.axp`). Open them in the Axoloti patcher and upload to the board.
