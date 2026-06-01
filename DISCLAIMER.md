# Disclaimer & provenance

## What this is
A **community-prepared Russian (ru) localization draft** for **Hellforged**, offered to the developers
to use, modify, or ignore freely. The goal is to make adding Russian as low-effort as possible for the team.

## How the strings were obtained
The English source strings and their localization **keys/ids** were read from the **shipped Hellforged
Playtest** build's Unity Localization string tables (the public `localization-*` AssetBundles), purely to
align the translation with the game's own `SharedTableData`. **No game code, art, audio, fonts, or other
assets are redistributed here** — this kit contains only:
- the localization **string keys/ids** (which the translation must reference to be importable), and
- the **English source text** (review aid) and a **Russian draft translation** of it.

## Quality / status
The Russian text is a **machine-assisted draft**, generated with a shared term glossary and automated
checks that placeholders (`{0}`, `{rewardAmount}`) and rich-text tags (`<sprite=…>`, `<style=…>`) are
preserved. It has **not** been reviewed by a professional human translator. Treat it as a strong starting
point, not a final localization. `QA_REPORT.md` lists any rows needing manual attention.

## Licensing intent
Provided **as-is**, without warranty, for the Hellforged developers. The underlying string keys and
English text are the property of the game's authors (studio “Solus”). The Russian translation draft is
contributed for incorporation into the game; the developers may relicense/edit it as needed. If you'd
prefer this material taken down or delivered differently, just say so.
