# Droplet music: the share-alike arrangements

Three of the chiptune arrangements from **Droplet**, an Android game by occupyjoshua. Each one is arranged from
an edition under a share-alike licence, so it is published here under that same licence. Each folder holds the
arrangement's note data (a Python file) and the audio files rendered from it, exactly as they ship in the game.
Droplet's code, art and other music are not part of this repository and are not covered by these licences.

| Folder | Piece | Arranged from | Licence |
|---|---|---|---|
| `shop/` | Alessandro Marcello / J. S. Bach, Adagio from the Concerto in D minor, BWV 974 | Melody: the public-domain Bach-Gesellschaft edition (Band 42, 1894, IMSLP #05913). Harmony: R. D. Tennent's edition for recorders, IMSLP #423014 | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) (`shop/LICENSE`) |
| `maple/` | Frédéric Chopin, Nocturne Op. 9 No. 2 | The Mutopia Project edition typeset by Renato Biolcati Rinaldi (2014, after G. Schirmer, 1881) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) (`maple/LICENSE`) |
| `station/` | W. A. Mozart (completed by F. X. Süssmayr), Lacrimosa from the Requiem K. 626 | Choral Public Domain Library edition CPDL #06799, full score typeset by Steve Jones | [CPDL License v4](https://www.cpdl.org/wiki/index.php/ChoralWiki:CPDL) (`station/LICENSE`) |

## What was changed

- **shop/**: the edition's MIDI was reduced to a melody line and the remaining voices, and bars 1-10 were set as
  Bach wrote them in the keyboard version. Arranged for chip voices by occupyjoshua, October 2026.
- **maple/**: the edition's MIDI was reduced to bass, chords, melody and inner voice, with its expression
  markings, and arranged for chip voices by occupyjoshua, October 2026.
- **station/**: changed by occupyjoshua on 8 October 2026: five of the edition's fifteen parts kept and reduced to
  note data for chip voices. Changed again on 9 October 2026: the edition's expression markings added.

The header of each Python file records its source and changes in more detail.

## The files

- `*.py`: the arrangement as note data (bars of `(beat, MIDI note, length)` events). It is read by the game's
  own renderer, which is not included.
- `*_run_*.ogg`: the layers that play together during a level (bass, left hand, lead, echo, harmony, drums,
  and the `_turn` variations). The game fades layers in and out as a level goes on.
- `*_menu.ogg`: the short loop on the menu. `*_sill.ogg`: the ending at the end of a level.

## Copyright and licence

Arrangements © 2026 occupyjoshua. Each folder is licensed under the licence in its own `LICENSE` file, the same
licence as the edition it was arranged from. Under those terms you may copy, share and adapt these arrangements;
credit the original edition and its editor as above, credit occupyjoshua for the arrangement, and share your
changes under the same licence.
