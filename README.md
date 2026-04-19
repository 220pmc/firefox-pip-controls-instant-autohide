# firefox-pip-controls-instant-autohide

Instantly hides Firefox Picture-in-Picture controls when not hovering — no fade, no delay.

## Features
- Controls are hidden when not hovering over the PiP window
- Controls appear instantly on hover
- Removes all fade animations and delays

## Caveats
- This CSS has only been tested on Firefox ESR 115

## Instructions

1. Enable `userChrome.css` support:
   - Open `about:config`
   - Set:
     ```
     toolkit.legacyUserProfileCustomizations.stylesheets = true
     ```

2. Open your profile folder:
   - Go to `about:support`
   - Find **Profile Folder**
   - Click **"Open Folder"**

3. Inside your profile folder:
   - Create a folder named `chrome` if it does not exist

4. Add the CSS file:
   - Place `pip_controls_instant_autohide.css` inside the `chrome` folder

5. Edit `userChrome.css`:
   - Create `userChrome.css` if it does not exist
   - Open it with any text editor
   - Add the following line:
     ```
     @import "./pip_controls_instant_autohide.css";
     ```

6. Restart Firefox
