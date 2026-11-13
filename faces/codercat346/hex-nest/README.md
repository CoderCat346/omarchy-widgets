# Hex Nest

Hex Nest is a full-page Omalauncher face that combines a theme-aware system dashboard with a gesture-driven nest of the apps you use most. It keeps the hexagonal feel of a command deck while launching apps the way Dragon Launcher does: drag toward an app, release, and it opens.

## Credit

This face is based on **[druspect](https://github.com/druspect)'s [Hex Command](https://github.com/SimonSchubert/omarchy-widgets/tree/main/faces/druspect/hex-command)**, the original. The command deck, the usage-ranked hex field and its theming are theirs; Hex Nest adds the gesture launching, the 1F/2F mode switch, pinch zoom and the collapsible deck. If you want the original, install Hex Command.

## First run

1. Install the face from the Omalauncher store, or copy `face.owl` into `~/.config/omalauncher/widgets/`.
2. Open the face — it sits left of your first home page.
3. Tap **1F LAUNCH** in the deck bar if it is not already selected.
4. Drag from the centre of the nest toward an app. The nearest app highlights as you move; let go to open it. Dragging back into the centre cancels.

The deck bar also has **2F VIEW**, zoom `+` / `−`, and **reset**. Tap **▾ COMMAND DECK** to collapse the system panel when you want more room for the nest.

## Gestures

### 1F LAUNCH (default)

- One finger drag: choose an app by direction and distance, then release to launch it.
- Tap an app: open it directly.
- The inner ring of six apps is drawn as a hexagon, not a circle.

### 2F VIEW

Use this when you want to inspect or rearrange the view rather than launch something.

- One finger drag: move the whole nest.
- Two fingers: pinch to zoom, and move both fingers to pan.
- Tap an app: still opens it.
- Press **reset** to return to 100% zoom and the centred position.

The mode toggle keeps one-finger launching and two-finger navigation from fighting each other. In 1F LAUNCH, gestures are reserved for launching; switch to 2F VIEW for zoom and pan.

## The command deck

The collapsible deck shows:

- Weather for the network's approximate location.
- Battery, memory, storage, CPU, display and thermal status.
- Notification and app-update counts.
- A nominal/attention state indicator.

Tap **▾ COMMAND DECK** to collapse it and give the nest the full page. Tap **▸ COMMAND DECK** to bring it back.

## Data and privacy

The face runs no shell commands and installs no packages. Weather is requested from `https://wttr.in/?format=j1`, which chooses an approximate location from the network request; no coordinates, account details or API keys are stored in the face.

The notification source is used only to display the local notification count. Notification contents are not rendered, written to disk or sent anywhere. App names, icons and usage scores stay inside Omalauncher and are used only to build the local ranking. Banking apps and Java runtime utilities are filtered out of the glanceable field.

## Compatibility

Hex Nest requires OWL 22 (Omalauncher 1.3.0 or newer). It is designed for phone-sized portrait faces and follows the active Omarchy theme, including light themes.

## Tips

- If launching feels too sensitive, use 2F VIEW and the **reset** button to recentre, then switch back to 1F LAUNCH.
- The app list is ranked by Omalauncher's own usage scores, so the apps you open most often move inward over time.
- The face is self-contained: it needs no Linux commands, packages or extra permissions beyond what Omalauncher already provides.

Suggestions and thoughtful review are welcome.
