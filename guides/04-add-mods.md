# 4. Add mods from Modrinth and CurseForge

Prism can search and download mods from **Modrinth** and **CurseForge** without opening a browser. It also picks the right file for your Minecraft version and mod loader.

## Download mods inside Prism (recommended)

1. Select your instance and click **Edit**.
2. Click **Mods** on the left, then **Download Mods**.
3. Choose **Modrinth** or **CurseForge** on the left.
4. Search for a mod, click it, then click **Select mod for download**. Repeat for every mod you want.
5. Click **Review and confirm**, check the list, and click **OK**.

Prism also offers to download a mod's **required dependencies** (like Fabric API or Cloth Config), so let it.

## "Some mods need to be downloaded manually" (CurseForge)

Some CurseForge authors don't allow other apps to download their files. When that happens, Prism shows a list of those mods with links:

1. Click each link and download the file from CurseForge in your browser.
2. Leave the Prism window open. It watches your **Downloads** folder and ticks each mod off (**Found**) as the file arrives.
3. When they're all found, click **OK**.

## Add a mod file you already downloaded

In **Edit → Mods**, drag the `.jar` file into the list, or use **Add file**. Only do this with files from sites you trust (see [Stay safe](07-safety.md)).

## Managing mods

- **Turn a mod off without deleting it**: untick the box next to it.
- **Update mods**: **Edit → Mods → Check for Updates**.
- **Remove a mod**: select it and click **Remove**.

## Rules that avoid most crashes

- The mod must match the **Minecraft version** *and* the **mod loader** of the instance. A Fabric mod won't load on NeoForge.
- Don't install the same mod twice (two versions of one mod = crash).
- Some mods don't mix. The classic example is **OptiFine** with **Sodium**. For shaders on Fabric, use **Sodium + Iris** instead of OptiFine.
- Add a few mods at a time and launch in between, so if something breaks you know which mod did it.

Next: [Install a whole modpack](05-modpacks.md)
