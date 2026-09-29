# 6. Fix common problems

## The game crashed. Where do I start?

1. Select the instance, click **Edit → Minecraft Log**.
2. Scroll to the bottom and look for the first line with **Caused by:** or **Exception**. The mod's name is often in it.
3. Still stuck? Click **Upload** at the bottom of the log page and share the link when asking for help, instead of screenshots.

## Common crash causes

| Message in the log | What it means | Fix |
|---|---|---|
| `Incompatible mods found!` / `requires ... which is missing` | A mod needs another mod you don't have. | Install the mod it names (often **Fabric API**). |
| `Missing or unsupported mandatory dependencies` | Same thing on Forge/NeoForge. | Install or update the mod named after `Mod ID:`. |
| `NoClassDefFoundError` | A required library mod is missing, or a mod is for the wrong loader/version. | Check each mod matches the instance's version and loader. |
| `OutOfMemoryError` | Minecraft ran out of RAM. | See below. |
| `class file version 65.0` (or similar) | Wrong Java version. | **Edit → Settings → Java**: turn automatic Java back on. |
| `Mixin apply for mod X failed` | Mod X doesn't fit this version or clashes with another mod. | Update or remove mod X. |
| `Found duplicate mods` | The same mod is installed twice. | Remove the older copy in **Edit → Mods**. |

## Not enough memory

1. Select the instance, **Edit → Settings → Java**.
2. Tick the **Memory** box, then set **Maximum memory allocation**.

Rough guide:

| Setup | Maximum memory |
|---|---|
| Vanilla or a few mods | 2–4 GB (2048–4096 MB) |
| Medium modpack (50–150 mods) | 4–6 GB |
| Big modpack (150+ mods) | 6–8 GB |

Don't give it more than about half your computer's RAM, and more than 8 GB rarely helps. It can even cause lag spikes.

## The game is slow

- On Fabric, add **Sodium**, **Lithium** and **FerriteCore**. On NeoForge, try **Embeddium** and **ModernFix**.
- Lower the render distance in Minecraft's video settings.
- Laptops: make sure Java uses your graphics card and the laptop is plugged in.

## I can't sign in

- Make sure the account owns Minecraft: Java Edition. Check at [minecraft.net](https://www.minecraft.net) → Profile.
- Remove the account in **Settings → Accounts** and add it again.

## Getting help

- [Prism Launcher wiki](https://prismlauncher.org/wiki/)
- The modpack's or mod's own page (Modrinth/CurseForge usually link a Discord or issue tracker).
- Always include your **uploaded log link**, the Minecraft version and the mod loader.

Next: [Stay safe when downloading mods](07-safety.md)
