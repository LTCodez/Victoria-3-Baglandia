# Baglandia

A Victoria 3 mod.

This repo was set up from the [Mod-Template](https://github.com/Victoria-3-Modding-Co-op/Mod-Template) by
Victoria-3-Modding-Co-op, with metadata and abbreviation (`BAG`) already filled in.

## Notes

- `mod/.metadata/metadata.json` `id` field is set to `com.github.LTCodez.baglandia`.
- Thumbnails (`mod/thumbnail.png`, `mod/.metadata/thumbnail.png`) and reference images in `image/` were not
  copied over automatically — grab those from the original template repo or replace with your own art:
  https://github.com/Victoria-3-Modding-Co-op/Mod-Template
- This folder currently lives directly inside your Victoria 3 `mod` directory. If you plan to push it to
  GitHub as a full repo (with `documentation/`, `image/`, `script/` etc.), consider moving the whole
  `Baglandia` folder somewhere outside the game's `mod` folder, then create a junction back to its `mod`
  subfolder so the Paradox Launcher only sees the actual mod content:

  ```
  mklink /j "C:\Users\<you>\OneDrive\Documents\Paradox Interactive\Victoria 3\mod\Baglandia-live" "C:\path\to\wherever\you\move\Baglandia\mod"
  ```

## Folder Structure

- `documentation/` — your mod's docs (not shipped to Steam)
- `image/` — reference art, templates, GIMP source files (not shipped to Steam)
- `mod/` — the actual mod content; this is what Paradox Launcher/Steam Workshop reads
- `script/` — helper scripts, e.g. `generate-localization.sh` to clone your English localization into
  other supported languages

## Further Resources

- Victoria 3 Wiki (Modding): https://vic3.paradoxwikis.com/Modding
- Victoria 3 Modding Co-op Discord: https://discord.com/invite/uUbuMTQjA7
