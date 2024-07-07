# Evil mods

#### Mods straight from hell

----------

This is the repository for modpacks, to be run with [evil-launcher](https://github.com/TheSmallTeaBoi/evil-launcher)

Please note that any file that isn't a `.hell` or `.md` can't be added to the
repo, this is to stop accidental inclusion of the actual WAD and mod files.

It is assumed you'll add your own `DOOM.WAD`, `DOOM2.WAD` and any other relevant
copyright-protected file to where they belong.

The file structure should be something like this:

```dirtree
Top level folder in repo
├─ /assets
│　├─ /wads
│　└─ /mods
│　　　├─ /maps
│　　　├─ /game
│　　　│　├─ /hdest
│　　　│　│　├─ /equipment
│　　　│　│　├─ /enemies
│　　　│　│　├─ /weapons
│　　　│　│　│　├─ /single
│　　　│　│　│　└─ /multiple
│　　　│　│　└─ /vehicles
│　　　│　└─ /reelism2
│　　　│　　　└─ /extensions
│　　　├─ /gameplay
│　　　└─ /other
└─ /hells
　　├─ /game1
　　├─ /game2
　　└─ /game3
```

- All hell files should go in `/hells`, with every game/modpack in a category.
    - It's nice to add a readme.md for every folder here, explaining what every
      hell file is

- Base game WADs, such as `DOOM.WAD` or `DOOM2.WAD` should go into `/assets/wads`

- All mods should point to `/assets/mods`, under a category:
    - `/maps` for map mods
    - `/game` for big mods, that have addons themselves
    - `/gameplay` for mods that change gameplay, but are otherwise fully
    compatible with other mods
    - `/misc` for mods that don't fit anywhere else
