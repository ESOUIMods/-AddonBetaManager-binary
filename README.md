# AddonBetaManager v1.0

Use this tool to download the latest beta or release versions of my ESO addons with one click.  

[Download AddonBetaManager](https://github.com/ESOUIMods/-AddonBetaManager-binary/releases/download/ver_3.0/AddonBetaManager_30.zip)

# AddonBetaManager Utility

AddonBetaManager is a small Windows utility that downloads and installs beta or release versions of selected Elder Scrolls Online addons directly into your AddOns folder. It is designed as a simple, safe way for users to test beta builds or quickly update supported addons without needing to download ZIP files manually.

## What It Does

- Downloads the latest **beta** or **release** versions of selected ESO addons
- Installs them directly into your AddOns folder
- Cleans the addon folder before installation to avoid leftover files
- Provides optional buttons for quick access to:
  - Master Merchant documentation
  - The author's Patreon page
  - Discord 
  - About Me (The Author)
  - The deleteLibStub cleanup tool
- Installs the deleteLibStub cleanup tool if requested
- Extracts ZIPs directly to the AddOns folder with no manual steps needed

AddonBetaManager does *not* replace Minion. Instead, it is meant to help with publishing beta builds for certain addons without requiring manual installation for testing.

## How to Use

1. Download the ZIP file from the Releases page.
2. Unzip it and place the executable anywhere you prefer (Desktop, Documents, etc.).
   - Unlike deleteLibStub, **AddonBetaManager does not need to be inside the AddOns folder**.
3. Double-click the EXE to run it.
4. For each supported addon, click either:
   - **Download beta** – installs the latest prerelease
   - **Download release** – installs the latest stable version
5. The status column will show progress messages during the download and installation process.

The utility downloads assets from GitHub Releases, extracts the ZIP, deletes the old addon folder, and installs the new version automatically.

## Supported AddOns

Support varies depending on which addons are maintained in the author's repositories. Typical examples include (but are not limited to):

- Master Merchant (MM)
- Alchemy Tooltips
- LibAlchemy
- Inventory Insight
- LibRecipe
- LibItemLink
- LibPrice
- WritWorthy
- TamrielTradeCentre Companion

Only addons with GitHub release or prerelease downloads are supported.

## Convenience Buttons

At the bottom of the tool, several optional buttons make it easier to access related resources:

### Patreon
Opens the author's Patreon page to support ongoing ESO addon development.

### MM Documentation
Opens the Master Merchant documentation website.

### deleteLibStub Tool
Downloads and installs the cleanup tool into the AddOns folder.  
This is helpful for fixing old embedded libraries in outdated addons.

### About / Discord
Provides links for contact, community help, or support channels.

## Install Location

By default, AddonBetaManager installs addons into:

C:\Users\<your user name>\Documents\Elder Scrolls Online\live\AddOns

If your ESO installation uses a custom or redirected AddOns folder, for now you will need to copy the folder from the standard location to where your Addons folder is located.

## If Files Do Not Appear in the AddOns Folder

Common reasons include:

- Windows Defender blocking the EXE from modifying files
- Running the tool from a protected folder (e.g., Program Files)
- Network issues when contacting GitHub’s API
- Incorrect permissions on the AddOns folder

See notes below for Windows Defender exceptions.

## Windows Defender / Permission Notes

If AddonBetaManager cannot create or delete files inside the ESO AddOns folder:

1. Open Windows Security.
2. Go to **Virus & threat protection**.
3. Scroll to **Ransomware protection**.
4. Click **Manage ransomware protection**.
5. If Controlled Folder Access is turned on:
   - Click **Allow an app through Controlled folder access**
   - Add AddonBetaManager.exe and/or deleteLibStub.exe

Then run the utility again.

## Updates and Feedback

AddonBetaManager improves over time as more addons are added and edge cases are resolved. If you experience issues or find that an addon is not installing correctly, you may open an issue on the repository or share details with the author.

## Disclaimer

- This tool does not update abandoned addons or fix broken Lua code.
- It only installs files from GitHub releases and cannot repair incompatible or out-of-date mods.
- Always backup your AddOns folder if you have highly customized setups.

Use the tool at your discretion and keep ESO mods up to date for best results.


