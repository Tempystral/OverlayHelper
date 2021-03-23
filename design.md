# Overview
Overlay Helper will be a Windows Forms application that allows a user to change and update resources in one convenient dialog. Fundamentally, the program will do little more than move around and rename files, but this is intended for use with tools like OBS, so it doesn't need to.

## Use Case
I run a livestream and sometimes want to update resources in my overlay such as images and text. However, it requires that I dig about in my layouts, selecting files one by one. OBS does not provide a way to make updating multiple items quick and seamless either. The alternative is to have multiple sources for each image or text object I want to change out, which makes navigating source lists more cumbersome.

## Design
### Main Window
The main window will have a single panel with multiple spaces for tiles, which begin blank. Each tile represents an overlay element which the user can edit. There is always a button in one tile to allow a user to add a new tile in that location. When a user clicks on a tile, a modal appears with controls to edit that tile's contents.

There will be a toggle which, when selected, allows the user to drag-and-drop tiles to rearrange their position in the interface. Selecting a tile normally is disabled in when this toggle is active.

Users can drag various media into the main window to immediately assign that file to a tile. If the content type does not match what the tile supports, it will be rejected.

## Tiles
Each tile contains controls for a specific type of media. A tile can be created for:
- Text
- Photos
- Videos
- more (?)
Each tile will present its name alongside either a thumbnail of the photo/video it contains or a sample of its text.

## Modal Window
When a user selects a tile, the modal which appears will provide the ability to edit the resource represented by that tile.
The window will display the name of the resource, its filename, a preview of the current media, and options (?)

- Should there be a file browser or database of some sort akin to Scoreboard Assistant?
