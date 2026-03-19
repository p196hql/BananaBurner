# BananaBurner Changelog - 2026-03-20

## Script v3.3
## Extension v2979.1.1

### Extension:
- CSP added to manifest.json HTTP & WS host perms removed
- Switched to cryptographic nonce
- Removed perm: declarativeNetRequestFeedback
- Other

### Script:
- Telemetry includes your quick actions on the dashboard, URL and servers can  be added as quick actions,  the script will now redact the action's server id and name,  same for url quick actions.
- modified initial security notice:
  - There's now a toggle to disable telemetry before you even enter the script on first launch.
  -  an example of the telemetry payload can be seen
  - added disclaimer about how you can request for your data  to be  deleted or ask for all of it (if not deleted)
- SRI verification for FontAwesome, Prism, Monaco
  - updated Prism (9000.0.1) and Monaco (0.53.0)
  - updated FontAwesome to 7.0.1
  - updated CodeJar to 4.3.0
  - removed prism tomorrow 
    - using atom dark & material light themes
- small UI improvements
- modified server details popup for phones
- modified pull out flags
- position changes for console and sidebar & flags
- layout improvements
  - market popup
  - server details popup
  - affiliates, webhooks tab in profile popup
  - other
- removed PiP console header
- url path now changes based on the tab you're on
  - based on the path, script will start on that tab
  - browser back/forward should trigger tab change
- ready toast removed
- coin collector fixes
- Light mode fix for console input
- CodeJar fix
- Some experimental stuff removed
- Bug fixes and improvements
- Other

Update by reinstalling the extension: https://discord.com/channels/884145104401608735/1476175295684939807/1476176972940841093

If there are any issues, let me know about it here!
-# Release #22 stable, some features are unavailable for userscript users.
Update by reinstalling the extension.

If there are any issues, let us know about it on Discord @agentzzrp or @paccman_0!<br>
Release #22 stable, some features are unavailable for userscript users.
