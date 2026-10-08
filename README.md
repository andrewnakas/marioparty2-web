# marioparty2-web

Mario Party 2 in the browser, bring your own ROM. Live at
https://andrewnakas.github.io/marioparty2-web/ and listed on https://decompgames.com.

**No game data is in this repository or on the page.** You pick your own ROM; it is read
in the tab and never uploaded.

## What this is

- **Source project:** [mariopartyrd/marioparty2](https://github.com/mariopartyrd/marioparty2) at `020a95ae0021a5d6d4e39cf98628cb86faba129a`.
- **Matching build:** All 421 C units plus the retained assembly were compiled with GCC 2.7.2 and a period GNU as; the linked 32 MiB ROM has SHA-1 `166eda1c05670d337e2c3f15a5db528ae1e5d6e3`, zero bytes different from the USA cartridge. The decompilation is partial: most functions are still included as assembly.
- **Browser player:** EmulatorJS 4.2.3 with the libretro Mupen64Plus-Next core (WebAssembly). This is emulation of the rebuilt ROM, not a native
  port of the game's code to WebAssembly.

## Tested

A Space Land round, the Tile Driver minigame through its results screen, a save-state restore and a cartridge-save round trip (muted). Audio has not been listened to: every test ran muted. Nothing
beyond that scope has been played.

## Layout

- `web/` — the page (published as the `gh-pages` branch).
- `web/THIRD_PARTY.md` — licences of the vendored runtime.
