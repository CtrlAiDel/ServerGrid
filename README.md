# ServerGridSync

**Author:** WeConnected  
**Version:** 4.8.0  
**Platform:** BetterDiscord (Discord desktop)

**ServerGridSync** adds a **Serv** button to Discord that opens a full-page grid of all your servers and folders. Drag and drop to organize them, and your changes are saved to your Discord account, so the left sidebar follows.

---

## ✨ Features

* **Full-page grid:** all your servers and folders on one page, in the same order as your Discord sidebar.
* **Drag and drop:** reorder servers and folders, and see an orange line showing exactly where they will land.
* **Synced with your sidebar:** every move is saved to your Discord account, so the left sidebar (and your other devices) match the grid.
* **Folders:** drop a server on another to create a folder, move servers in and out of folders, rename or dissolve folders.
* **Right-click menu:** open a server, move it left or right, remove it from a folder, hide it from the grid, or leave the server.
* **Open folders / Close folders:** expand or collapse every folder at once. Big folders flow into columns.
* **Hidden servers:** hide servers from the grid only, and bring them back with one click.
* **Status badges:** unread dots and mention counts, and your current server is highlighted.
* **Backup:** a copy of your folders is saved before the first change, so you can undo.

---

## 📥 Installation

1. Download `ServerGridSync.plugin.js`.
2. In Discord, open **User Settings** → **Plugins** (BetterDiscord section) → **Open Plugins Folder**.
3. Put `ServerGridSync.plugin.js` directly in that folder (no subfolder).
4. Go back to Discord and switch **ServerGridSync** on.

> Keep only one ServerGrid plugin enabled. Older versions add the same **Serv** button.

---

## 🚀 Usage

1. Click the **Serv** button, in the left sidebar under Direct Messages.
2. **Reorder:** drag a server or folder and drop it near the edge of another tile. The orange line shows where it will go.
3. **Create a folder:** drop a server in the middle of another server.
4. **Add to a folder:** drop a server in the middle of a folder.
5. **Take out of a folder:** drag it between two tiles on the main line, or into empty space, or use **Remove from folder** in the right-click menu.
6. **Open folders / Close folders** (bottom right) expand or collapse every folder.
7. Click a server to jump straight to it. Use the red **✕** at the top right to close the grid.

---

## ⚙️ Settings

Settings → Plugins → ServerGridSync:

* **Servers per column in an open folder**
* **Icon size**
* **Restore backup:** puts your folders back as they were before the plugin's first change.

---

## 🛠️ Troubleshooting

* **The plugin isn't showing up:** the file must be named exactly `ServerGridSync.plugin.js` (no `(1)` added by your browser) and sit directly in the `plugins` folder. Restart Discord afterwards.
* **The sidebar didn't change:** a notice appears a few seconds after a move and tells you what Discord answered. It is also copied to your clipboard. Reload Discord (Ctrl+R) and check again.
* **Undo a change:** use **Restore backup** in the plugin settings.
* **Custom folder icons:** if the plugin can't read your Discord settings before saving, folder extras like custom icons may be reset.
* **Style conflicts:** if you use themes or plugins that heavily change the server sidebar, disable them temporarily to check.
