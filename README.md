# ServerGridSync

**Author:** WeConnected  
**Version:** 5.0.0  
**Platform:** BetterDiscord (Discord desktop) / Javelic0rd (Alternative Discord software)

## What it does

ServList adds a **Serv List** button to your Discord sidebar (right under *Direct Messages*). It opens a full-page grid of every server and folder you have, in exactly the same order as your sidebar. Move things around on the page and your real sidebar follows.

## Features

- **Full-page grid:** all servers and folders on one line that wraps, in your sidebar's order.
- **Drag and drop:** an orange insertion line shows exactly where a server or folder will land.
- **Folders like Discord's:** drop a server on another to create a folder, drop it on a folder to add it, drag it out to remove it.
- **Synced with Discord:** every change is saved to your Discord account, so the sidebar (and your other devices) match.
- **Right-click menu:** open a server, move it left or right, remove it from a folder, hide it from the grid, leave the server. Folders can be renamed, moved or dissolved.
- **Open folders / Close folders:** expand or collapse every folder at once. Big folders flow into columns.
- **Hidden servers:** hide servers from the grid only, and bring them back with one click.
- **Badges:** unread dots and mention counts, and your current server is highlighted.
- **Backup:** your folders are saved before ServList's first change, so you can undo.
- **Safe saving:** nothing is sent to Discord if a server would be duplicated or missing.

## Requirements

- Discord desktop with [BetterDiscord](https://betterdiscord.app/) installed.
- A recent version of Discord (the page uses the browser's top-layer *Popover API*).

## Installation

1. Download [`ServList.plugin.js`](ServList.plugin.js).
2. In Discord, open **User Settings → Plugins** (BetterDiscord section) → **Open Plugins Folder**.
3. Put `ServList.plugin.js` directly in that folder (no subfolder).
4. Go back to Discord and switch **ServList** on.

> **Upgrading from ServGrid / ServerGridSync?** Delete the old plugin file and keep only one of them enabled. ServList imports your old settings, hidden servers and open folders the first time it runs.

## Usage

| I want to… | Do this |
|---|---|
| Open the grid | Click the **Serv List** button in the left sidebar |
| Open a server | Click it |
| Reorder | Drag a tile and drop it near the edge of another tile (follow the orange line) |
| Create a folder | Drop a server in the **middle** of another server |
| Add to a folder | Drop a server in the middle of a folder |
| Take out of a folder | Drag it between two tiles on the main line, or into empty space, or use **Remove from folder** in the right-click menu |
| Expand / collapse folders | **Open folders** / **Close folders** (bottom right) |
| Close the grid | The red **✕** at the top right (or `Esc`) |

## Settings

*Settings → Plugins → ServList*

- **Servers per column in an open folder**
- **Icon size**
- **Restore backup:** puts your folders back as they were before ServList's first change.

## How the sync works

Discord stores your server order and folders in your account settings. ServList reads them through Discord's own client connection and, when you move something, writes the new order back the same way. Before the first change it saves a backup of your current layout (see **Restore backup**). If the sidebar doesn't change after a move, a notice appears a few seconds later and shows what Discord answered. The text is copied to your clipboard so it can be pasted into an issue.

## Troubleshooting

- **The plugin doesn't show up:** the file must be named exactly `ServList.plugin.js` (browsers sometimes add `(1)`) and sit directly in the `plugins` folder. Restart Discord afterwards.
- **The sidebar didn't change:** reload Discord (`Ctrl+R`) and look again. If a notice appeared, copy its text into an issue.
- **A server won't open from a folder:** ServList tries several ways in turn and, if all fail, shows a details window (also copied to your clipboard). Please include that text in an issue.
- **Undo a change:** use **Restore backup** in the plugin settings.
- **Custom folder icons got reset:** if ServList can't read your Discord settings before saving, folder extras such as custom icons can't be kept. The notice says when this happened.
- **Style conflicts:** with themes or plugins that heavily change the server sidebar, disable them temporarily to check.
- **Logo not lined up:** it aligns itself with Discord's Home button; resizing the window re-aligns it.

## Disclaimer

Client modifications are not supported by Discord and may go against its Terms of Service. Use ServList at your own risk. It is not affiliated with or endorsed by Discord or BetterDiscord.

## Changelog

**5.0.0**
- Renamed to **ServList**, with a new "Serv List" logo (transparent background, aligned with the other server icons).
- Imports settings from ServGrid / ServerGridSync.
- More reliable opening of servers inside folders, with a details window if it still fails.
- Keeps Discord's old server-order list consistent when saving.
- The page switches back to the sidebar's real order, with an explanation, if a save didn't go through.

**4.x** – Sync with the Discord sidebar, folders by drag and drop, Open/Close folders, backup and restore.
**1.x – 2.x** – First versions: full-page grid, drag and drop reordering, local folders.

## Author

**WeConnected**
