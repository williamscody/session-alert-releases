# Session Alert

A tiny Mac menu bar app for musicians who share Logic Pro projects over iCloud Drive.
When you open a project from your shared folder, Session Alert puts a lock file right under it in Finder
(`Song.logicx 🔒 in use by Bill.sessionlock`). If your collaborator opens the same song while it's locked,
a window pops up telling them you're in it, so you never work on the same song at the same time.
The lock is removed when you close the project (or quit Session Alert), and they get a notification that it's free.

When your collaborator has a song open, Session Alert also tags it **orange** in Finder on your Mac,
and removes the tag once they close it.

## Install

1. Download the latest `Session-Alert-x.y.zip` from [**Releases**](../../releases/latest) and unzip it.
2. Drag **Session Alert** into your **Applications** folder and open it
   (replace the old copy if you're updating). A music-note house icon appears in the menu bar.
3. **Allow Accessibility access** when asked (System Settings › Privacy & Security › Accessibility),
   then quit and reopen Session Alert. This lets it read which song Logic has open.
   If you're updating and it keeps asking, remove Session Alert from that list and add it again.
4. Allow notifications when asked.
5. Click the menu bar icon › **Settings…** and:
   - enter your name as it should appear on lock files
   - choose your **shared folder** (the iCloud Drive folder with your projects)
   - check **Watched apps**: Logic Pro is there by default; use **Add Running App** or
     **Choose App…** to add others
   - turn on **Launch Session Alert at login**

Requirements: macOS 14 or later. Both collaborators need to install it, pointed at the same shared folder.
