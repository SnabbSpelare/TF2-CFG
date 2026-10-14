# Team Fortress 2 – Configuration – Public Build [release]

## Description

I am creating a stable, easy-to-use version of my personal configuration. This build focuses on clarity and simple customization. More updates will follow soon.

## Table of Contents

- [Hidden console commands](#-hidden-console-commands)
- [Removed console commands](#-hidden-console-commands)
- [Configuration Warnings](#️-configuration-warnings)

### 🔒 Hidden console commands

`mat_forcemanagedtextureintohardware 0`

`mat_parallaxmap 0` — ⚠️ May crash and cause temporary stuttering. [See Configuration Warnings](#️-configuration-warnings)

### 🗑️ Removed console commands

`cl_forcepreload` — Use `sv_forcepreload 0` instead.

### Common Misconceptions

Placed in order of most importance to least clarification.

#### def. Values Are Not Always the Actual Defaults

Some def. values are not the actual default values for the current version of the game. They may be left over from older branches or simply never updated, they do not reflect settings todays Valve.

Because of this, you should not assume that a def. value is accurate. In many cases, it is only a suggestion and may differ from the actual default.

For this reason, **write down the current value before changing them.** This gives you a reliable way to restore your original settings.

To find the actual defaults for the current version, restart the game with the `-default` launch option. In TF2, this forces the game to use its default settings and overrides configuration files and manually entered console commands.

#### mat_hdr_enabled is not how to change HDR

`mat_hdr_enabled` **vs.** `mat_hdr_enable`

`mat_hdr_enabled` is often confused with `mat_hdr_enable`, an older command that was removed in Source 2007. `mat_hdr_enabled` is a debugging command used to report whether the current map has HDR enabled.

Using either command with 0 or 1 is **not valid or supported in TF2.** To change the HDR, use `mat_hdr_level 2` instead.

#### ⚠️ Configuration Warnings

Some settings may cause crashes or temporary stuttering after being changed. Wait a few seconds for the renders to finish refreshing before continuing.
