# Texture Wrangler for Blender

Texture Wrangler copies texture map files into material folders and renames them to a consistent naming convention, so `Brass_NormalGL.png` becomes `brass001_normal.png` without renaming each file by hand.

It was built to add your own materials to the **MaterialWorks** library, which expects specific file names, but it works just as well on its own to keep any texture collection organized.

> This repository is for **bug reports, feature requests and questions**. The add-on's source code is not hosted here.

## Download and install

Install Texture Wrangler from the Blender Extensions Platform:

**https://extensions.blender.org/add-ons/texture-wrangler/**

Or install from inside Blender:

1. Open **Edit > Preferences > Get Extensions**.
2. Search for **Texture Wrangler** and click **Install**.

Installing from the platform means Blender will let you know when an update is available.

**Requires Blender 4.2 or newer.**

## Where to find it

In the 3D Viewport, press **N** to open the sidebar and select the **TextureWrangler** tab.

## How it works

1. **Pick a source folder** that holds the texture files for one material.
2. Texture Wrangler finds the material's root name and works out which map each file is (normal, roughness, base color, and so on).
3. **Rename the material** if you like. Change `Brass4KFromMike` to `brass001` and every output file follows.
4. **Fix any file it couldn't identify** by choosing its type from the list. Click the bookmark icon to save that name as an association, so the file is recognized automatically next time.
5. **Copy to 1K or Copy to 4K.** The files are copied into the output folder under their new names. Your source files are never changed or moved.

### Other features

- **Name Associations panel**: view, add and remove the names that are matched to each map type.
- **Texture Utilities > Organize Materials**: split a folder that contains many materials into one subfolder per material.
- **Image preview**: view a texture before you copy it.
- **Copy history** (optional): records each copy in `texture_wrangler_history.txt` in the output folder.
- **Saved file names**: change the suffix each map type is saved with in **Edit > Preferences > Add-ons > Texture Wrangler**.

## Reporting a bug

Open a [new issue](../../issues/new/choose) and choose **Bug report**. The form asks for:

- Your Blender version (**Help > About Blender**)
- Your Texture Wrangler version (**Edit > Preferences > Add-ons > Texture Wrangler**)
- Your operating system
- The steps that cause the problem
- The names of the texture files involved, if the problem is about how files are identified or renamed
- Any error message. On Windows, open **Window > Toggle System Console** to see errors. On macOS and Linux, start Blender from a terminal and the errors appear there.

Please search the [existing issues](../../issues) first, in case someone has already reported it.

## Requesting a feature

Open a [new issue](../../issues/new/choose) and choose **Feature request**. Describe what you are trying to do. That helps more than a description of a specific solution.

## Questions

For "how do I…" questions, use [Discussions](../../discussions) rather than Issues.

## License

Texture Wrangler is licensed under the GNU General Public License v3.0 or later.

---

Created by Eric Zwirnmann (Cowwolfe3D)
