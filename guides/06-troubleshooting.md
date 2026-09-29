# 6. Fix common problems

## 💥 The game crashed. What now?

### Step 1: Open the log

1. In the main window, click the instance **once**.
2. Click **Edit...** on the right.
3. In the list on the left, click **Minecraft Log** (it's the very first item).

### Step 2: Find the problem line

1. Scroll to the **bottom** of the log.
2. Scroll **up** slowly until you see red text or a line that starts with **`Caused by:`** or contains **`Exception`** or **`Error`**.
3. Look at the table below. Press **Ctrl + F** (Mac: **Cmd + F**) in your browser to search this page for a word from your error.

| If the log says... | It means... | Fix it like this |
|---|---|---|
| `Incompatible mods found!` or `requires ... which is missing!` | A mod needs another mod you don't have. | Read the line: it names the missing mod. Install it with **Download Mods** ([guide 4](04-add-mods.md)). Very often it's **Fabric API**. |
| `Missing or unsupported mandatory dependencies` + `Mod ID: 'something'` | Same thing, on Forge/NeoForge. | Install the mod called *something*. |
| `NoClassDefFoundError` or `ClassNotFoundException` | A needed mod is missing, **or** a mod is for the wrong loader/version. | Check every mod is for your instance's version **and** loader. If it mentions `fabricmc.fabric`, install **Fabric API**. |
| `java.lang.OutOfMemoryError` | Minecraft ran out of RAM. | [Give it more memory](#not-enough-memory). |
| `class file version 65.0` (or 61.0, 69.0...) | Wrong Java version. | [Turn on automatic Java](#wrong-java). |
| `Mixin apply for mod XYZ failed` | Mod *XYZ* doesn't fit this Minecraft version, or fights with another mod. | Update or remove mod *XYZ*. |
| `Found duplicate mods` | The same mod is installed twice. | On the **Mods** page, delete the older copy. |
| `Pixel format not accelerated` / `OpenGL` | Your graphics driver is old. | Update it from the NVIDIA, AMD or Intel website. |

### Step 3: Still stuck? Ask for help the right way

1. On the **Minecraft Log** page, click **Upload** at the bottom.
2. Prism gives you a **link**. Copy it.
3. When asking for help (the mod's Discord, a forum, a friend), send:
   - the **link** (not a screenshot!)
   - your **Minecraft version** and **mod loader**
   - what you did right before it broke

---

## Not enough memory

Big modpacks need more RAM than the default.

1. Click the instance **once**, then **Edit...**.
2. In the list on the left, click **Settings** (near the bottom).
3. At the top of that page, click the **Java** tab.
4. Find the **Memory** box and **tick its checkbox** so you can change it.
5. Change **Maximum Memory Usage** to:

   | Your setup | Set it to |
   |---|---|
   | No mods / a few mods | **4096 MiB** |
   | Medium modpack (50–150 mods) | **6144 MiB** |
   | Huge modpack (150+ mods) | **8192 MiB** |

6. Close the window. It saves by itself.

⚠️ Never use more than **half** of your computer's RAM. (Windows: **Settings → System → About** shows it. Mac: ** → About This Mac**.) More than 8192 rarely helps and can cause lag spikes.

## Wrong Java

1. Click the instance **once**, then **Edit...** → **Settings** → **Java** tab.
2. **Untick** the **Java Installation** box. That makes the instance use Prism's automatic Java again.
3. Launch again. Prism downloads the right Java if needed.

If that doesn't help: main window → **Settings** → **Java** → make sure **Auto-download Mojang Java** is ticked.

## The game is laggy

- **Fabric:** add **Sodium**, **Lithium** and **FerriteCore** (search them in **Download Mods**).
- **NeoForge / Forge:** add **Embeddium** and **ModernFix**.
- In the game: **Options → Video Settings** → lower **Render Distance** to 8–12.
- Laptop: plug it in, and close Chrome/Discord while playing.

## I can't sign in / "you don't own Minecraft"

1. Main window → **Settings** → **Accounts**.
2. Click your account → **Remove**.
3. Click **Add Microsoft** and sign in again with the email that **bought** Minecraft ([guide 2](02-sign-in.md)).

## The launcher itself won't open

- Restart your computer and try again.
- Reinstall Prism from **prismlauncher.org/download**. Your instances are kept.
- Still broken? Read the [Prism Launcher wiki](https://prismlauncher.org/wiki/) or ask on their Discord.

➡️ Next: [Stay safe when downloading mods](07-safety.md)
