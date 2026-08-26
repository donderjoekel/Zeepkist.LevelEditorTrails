# Zeepkist-LevelEditorTrails

A mod that draws trails in the level editor for completed test runs.
The trails show the path of each test run.
The trails help you place the next blocks.

## Installation

Install LevelEditorTrails with [Modkist](https://github.com/Thundernerd/ModkistMKII).
Modkist installs BepInEx and ZeepSDK.

## How to use

LevelEditorTrails records each test run in the level editor.

To record a trail:

1. Open the level editor in Zeepkist.
2. Click the test button, or press the test key.
3. Play the level. The mod records a trail during the test run.
4. After you finish the test run, return to the editor. The editor shows the trail.

Each extra test run adds a trail.
The trails show different paths.

### Controls

Default keys:

- **F7**: This key shows or hides all trails.
- **F6**: This key shows or hides the time markers.
- **F8**: This key removes all recorded trails.

## Config

You can edit the config file of LevelEditorTrails.
The config file is at `BepInEx/config/LevelEditorTrails.cfg`.

You can edit this file with a text editor.
You can also edit the config in the game with Zeep mod settings.

### Config keys

#### General

| Key                | Default value | Description                                                                                          |
|--------------------|---------------|------------------------------------------------------------------------------------------------------|
| Maximum Recordings | 5             | The mod keeps this many trails in memory. When the count gets to this limit, the mod removes the oldest trail. |
| Trail Width        | 0.5           | The width of the trail line is between 0.1 and 2. A larger value makes a thicker line. |
| Draw Time Markers  | true          | If Draw Time Markers is true, the mod shows time markers on the trails.                              |
| Time Marker Step   | 1.0           | This value is the time in seconds between time markers.                                              |

#### Keyboard Shortcuts

| Key                           | Default value | Description                                    |
|-------------------------------|---------------|------------------------------------------------|
| Toggle Line Visibility        | F7            | This key shows or hides all trails.            |
| Toggle Time Marker Visibility | F6            | This key shows or hides the time markers.      |
| Remove All Lines              | F8            | This key removes all recorded trails.          |

#### Colors

| Key         | Default value | Description                                                                              |
|-------------|---------------|------------------------------------------------------------------------------------------|
| Color Mode  | Gradient      | This is the color mode for the trails. `Single` uses one color for all trails. `Gradient` changes the color from the newest trail to the oldest trail. |
| Color       | White         | If Color Mode is `Single`, all trails use this color.                                    |
| Start Color | White         | If Color Mode is `Gradient`, the newest trail uses this color.                           |
| End Color   | Black         | If Color Mode is `Gradient`, the oldest trail uses this color.                           |
