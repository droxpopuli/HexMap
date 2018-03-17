# HexMap
A GDscript based hex library with storage and helper functions.

To use in your own project stick the HexMap folder in addons at the top level of your project folder. In Project Properties enable the plugin. The new HexMap Node will be available to use.

# Usage
```
Public properties
var is_flat: Determines drawing style of flat or pointy topped hex
var size: A Vector2 of given hex size. x doesnt not have to equal y
var origin: The x/y position of the origin of the grid

func add_hex(hex, data): Add new data to an unoccupied hex.
func move_hex(hex_old, hex_new): Move occupied hex to unoccupied location.
func remove_hex(hex): Remove an occupied hex
func get_hex(hex): Get data for a hex
func get_all_hex(): Get a dict of all hex data
func get_wall(hex, direction): Get wall data for a given hex

Rotation Transform Herlpers
func rotate_hex_left(hex):
func rotate_hex_right(hex):

Pixel funcs and things useful to drawing.
func hex_to_pixel(hex): x,y for a given hex..
func pixel_to_hex(pos): Full hex for a given x,y
func round_hex(hex): Round fractional hex to full.
func hex_corner_offset(corner): Vector2 Offset for a given corner based on layout
func hex_corners(hex): Array of Vector2 locations to draw a full hex.

Neighbor and Distance Utility Functions
func neighbor_hex(hex, direction):
func diagonal_neighbor_hex(hex, direction):
func hex_length(hex):
func hex_distance(hex_a, hex_b):
```

Credit to RedBlobGames for their Hex Map Resources.
