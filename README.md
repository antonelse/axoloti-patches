# axoloti-patches

Patches for the [Axoloti](https://ksoloti.github.io/2-background.html) DSP environment, by Johannes Taelman.

**Tested hardware:** Axoloti Core v1.2. Ksoloti, the successor platform, is not tested. Objects are not always compatible between the two, so check before porting.

## Contents

| Patch | Folder | Latest | Description | Controller |
|-------|--------|--------|-------------|------------|
| AnDrone | [`androne/`](./androne) | v2.1.0 | Six-oscillator drone synth, inspired by Guilherme Martins' Drone Engine. Scale quantisation, 3x3 matrix mixer, piezo line input. | M-Audio UC33e, presets P23–P25 in [uc33e-mappings](https://github.com/antonelse/uc33e-mappings) |
| AxoGlitch | [`axoglitch/`](./axoglitch) | v5 | Glitch processor. | Korg nanoPAD (mapping not yet written) |

`.axp` files are Axoloti patcher projects: open them in the Axoloti patcher and upload to the board.

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

## TODO

- [ ] AxoGlitch: write the guide and changelog
- [ ] AxoGlitch: write the nanoPAD mapping
- [ ] AxoGlitch: GlitchBeast effects with MIDI tempo sync
- [ ] AnDrone: open items listed in [`androne/GUIDE.md`](./androne/GUIDE.md)
- [ ] Ksoloti: test AnDrone and AxoGlitch, or keep them marked as Axoloti Core only

## License

GPL-3.0. See [LICENSE](./LICENSE). AnDrone derives from Guilherme Martins' Drone Engine, which is also GPL-3.0.
