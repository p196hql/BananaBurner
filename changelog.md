# BananaBurner Changelog - 2026-03-18

## Script v3.2
## Extension v2979.1.0

### Transparency:
Replaced obfuscated Injected.js with the original, while this may open opportunities for malicious people to make evil copies of BananaBurner, it's the optimal move from my side to avoid accusations of evil intent. Be advised to confirm you got the extension from github.com/relentiousdragon

My original intention was to protect the script from modifications and redistribution of malicious copies.

### New Stuff:
**Extension:**
- Commented out console logs to keep the  console clean, these are proxyFetch logs and other stuff, you can still view proxyFetch by inspecting the extension's popup and heading over to the network tab.
- reviewed security details and modifications for new market.
- Removed force inject button from popup
- Modified manifest
- Other 
---
**Script:**
- Organized console logs
**SERVER DETAILS:**
- Startup Settings:
  - Git Plugin @paccman_0:
    - when saving startup settings, git plugin will now automatically update the entry point in bb-github.sh to reflect your startup file's path.
    - When saving, save button is disabled until all plugins (if any installed) have 
completed their work.
    - fixed git plugin not fetching the right startup variables for startup  file on nodejs and python servers.
- File Explorer:
  - modified icons  for actions
  - layout adjustments
  - Reload button (CMD/CTRL + R)
    - Reloads the current directory, if you have VFS enabled and your code itself makes/deletes files, it may still be cached in  the VFS so you might have to reload the current directory, if you have VFS disabled you shouldn't have to worry about this, the button is there either way.
   - Shortcut keys: (CTRL = CMD on MacOS)
     - CTRL + SHIFT + I : Create new folder
     - CTRL + I : Create new file
     - DELETE (When files/folders are selected via CTRL + L-CLICK) : Delete files/folders
- Fixed bugs with template deployment when   VFS is enabled
- Fixed VFS bugs
- Root directory will always be rescanned in background to check for new files if VFS is enabled
- Fixed bug with shared servers that  are suspended
   - "Details" button is disabled for suspended shared servers
   - Fixed UI bug for shared servers that are suspended
- Modified telemetry data, fixed bugs with telemetry data disappearing randomly.
- When managing subusers, if you own the server, you will be able to assign all permissions, but if you don't, you will only be able to assign subusers you add the permissions you already have, that is if you have permission to create subusers on the server
- Added subuser perm for reading activity logs
  -  this is only for when you invite a subuser, at the moment you can't view activity logs for a server, this may be added in a future update
- Reduced unnecessary re-renders of dashboard.
- Other
**PLUGIN FRAMEWORK**:
- All plugin event listeners can be `async` functions. The framework will wait for all plugin listeners to resolve before proceeding with certain UI actions.
- Saving Startup Variables fires an event.
- Widget fixes and improvements
- Logger
- Documentation updates
- Other
**DEVELOPER UPDATES**
As a plugin developer, you will now have access to tools for testing and helping with your plugin development.
- DEVELOPER MODE:
   - To enable developer mode, open your browser's devtools console on the page and enter this command: 
      - BananaBurner.setDevMode(true)
   - DEVELOPER MODE allows you to load local plugins into the script, make sure you only load plugins you trust
   - Access to tools and features to help aid plugin development
   - Local Loaded plugins show up in the Market tab -> "Local"
- Added security notice for opening devtools console when DevMode is disabled.
- UI adjustments
- Modified reset local storage logic
- Bug Fixes and improvements
- Other

The Git plugin now requires script v3.2 to work, if you're on an older version, you will not be able to install and enable it. 
*Plugins: bot-id & bulk-server-manager also require v3.2 now.*

To update a plugin, you have to right click -> uninstall it, then install it again from the Market.

You can request for all telemetry data by sending me a DM, all previous telemetry data is no longer with Termux Labs so this counts for telemetry data from Match 18th and onwards.

Update by reinstalling the extension.

If there are any issues, let us know about it on Discord @agentzzrp or @paccman_0!<br>
Release #21 stable, some features are unavailable for userscript users.
