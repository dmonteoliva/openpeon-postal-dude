# openpeon-postal-dude

Postal Dude sound packs for [peon-ping](https://github.com/PeonPing/peon-ping) —
your coding agent reacts with voice lines from POSTAL 2.

Two packs live in this repo:

| Pack | Clips | Flavour |
|---|---:|---|
| [`postal-dude`](./postal-dude/) | 62 | Uncensored. The Dude swears. |
| [`postal-dude-clean`](./postal-dude-clean/) | 54 | Same pack, profanity removed. |

Both cover all 9 CESP v1.0 categories.

## Install

```bash
peon packs install postal-dude        # or postal-dude-clean
peon packs use postal-dude
```

No registry, straight from a clone:

```bash
git clone https://github.com/dmonteoliva/openpeon-postal-dude.git
peon packs install-local openpeon-postal-dude/postal-dude
peon packs use postal-dude
```

## Layout

```text
postal-dude/          uncensored pack
  openpeon.json       CESP v1.0 manifest
  sounds/             62 mp3 clips
postal-dude-clean/    profanity-free pack
  openpeon.json
  sounds/             54 mp3 clips
AUTHOR.md             guide for authoring your own pack
```

Each pack is registered separately in the OpenPeon registry, sharing this
repo and git tag via distinct `source_path` values.

## License

[CC BY-NC 4.0](./postal-dude/LICENSE) on the curation, editing, and manifests.
The voice recordings are from POSTAL 2, (c) Running With Scissors, Inc., and
remain the property of their rights holders — see any pack's `LICENSE` for the
full scope.
