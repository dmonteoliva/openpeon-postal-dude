# Postal Dude (POSTAL 2)

The Postal Dude from POSTAL 2 reacts to your coding session. Uncensored.

This is the **uncensored** pack — the Postal Dude swears. For a profanity-free cut, see [`postal-dude-clean`](../postal-dude-clean/).

## Install

From the OpenPeon registry:

```bash
peon packs install postal-dude
peon packs use postal-dude
```

Or straight from a local clone, no registry needed:

```bash
git clone https://github.com/dmonteoliva/openpeon-postal-dude.git
peon packs install-local openpeon-postal-dude/postal-dude
peon packs use postal-dude
```

## Contents

62 clips across all 9 CESP categories.

| Category | Clips | Fires when |
|---|---:|---|
| `session.start` | 7 | CLI launches / new session begins |
| `task.acknowledge` | 7 | Agent accepted work, processing started |
| `task.complete` | 9 | Work finished successfully |
| `task.error` | 8 | Something failed |
| `input.required` | 7 | Blocked waiting for user input or approval |
| `resource.limit` | 6 | Rate limit, token limit, or quota hit |
| `task.progress` | 7 | Long-running task heartbeat |
| `session.end` | 5 | Session closes gracefully |
| `user.spam` | 6 | User sending commands too rapidly |

### A note on coverage

This pack covers every category the [CESP v1.0 spec](https://openpeon.com/spec)
defines. Note that peon-ping 2.29.0 only routes seven of them: `session.end`
is received but used for state cleanup without playing audio, and no CLI
adapter currently emits `task.progress` at all. Those two are included so the
pack works unchanged if and when host support arrives.

## Audio

Source clips are 22 kHz mono PCM WAV, ripped from the game. Each was
loudness-normalised (`loudnorm I=-16 TP=-1.5 LRA=11`) and encoded to mono
44.1 kHz MP3 (VBR q5) so no clip is jarringly louder than another.

Clips run roughly 0.5–5 seconds.

## Credits

Voice: Rick Hunter as the Postal Dude.
Game: POSTAL 2 (c) Running With Scissors, Inc.
Transcripts and source audio: the [POSTAL Wiki](https://postal.fandom.com/wiki/Postal_2-_Postal_Dude_Voice_Lines).

Pack assembled by [@dmonteoliva](https://github.com/dmonteoliva).

## License

[CC BY-NC 4.0](../LICENSE) — covering the curation, editing, and manifest.
The underlying voice recordings remain the property of their rights holders.
See [`LICENSE`](./LICENSE) for the full scope.
