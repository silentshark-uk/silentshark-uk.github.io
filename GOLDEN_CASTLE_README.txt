THE GOLDEN CASTLE — Browser Conversion
======================================

Original game
-------------
The supplied golden.prg is a 19 KB Commodore 64 BASIC V2 program containing
532 BASIC lines. It defines a 66-location text adventure with 29 objects,
verb–noun commands, puzzles, enemies, scoring, instructions, and save/load
routines.

Browser edition
---------------
Open golden_castle_browser.html in a modern browser. It is a single,
self-contained HTML file: no installation, server, emulator, or internet
connection is required.

Useful commands include:
  NORTH / SOUTH / EAST / WEST / UP / DOWN
  LOOK
  INVENTORY
  GET TORCH
  LIGHT MATCHES
  LIGHT TORCH
  EXAMINE BOOK
  GIVE GOLD
  SCORE
  SAVE
  LOAD
  RESTART
  INSTRUCTIONS

SAVE normally uses browser local storage. If a browser blocks storage for a
locally opened HTML file, an in-page fallback still allows SAVE and LOAD until
the page is closed.

Preservation notes
------------------
The room descriptions, map connections, initial object positions, noun and
verb vocabulary, puzzle logic, encounters and original wording were recovered
from the tokenised PRG.

This is a JavaScript adaptation rather than a full C64 emulator. Input handling
is more forgiving than the 1987 version and supports additional natural aliases.
Two evident original BASIC defects were corrected:
  * The listed 150-point maximum was unreachable because the raft awarded 19
    points; the browser edition awards 20.
  * The buried-paper discovery can now occur only once.

Files
-----
golden.prg                 Original uploaded Commodore program
golden_detokenized.bas     Human-readable BASIC source recovered from the PRG
golden_castle_browser.html Standalone playable browser adaptation
golden_castle_preview.png  Preview image

This is an initial preservation build and should be play-tested against the
original for any obscure behavioural differences.
