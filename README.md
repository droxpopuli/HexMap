# HexMap
A GDscript based hex library with storage and helper functions.

To use in your own project stick the HexMap folder in addons at the top level of your project folder. In Project Properties enable the plugin. The new HexMap Node will be available to use.

# Usage
```
Public properties
var is_flat
var size
var origin

Add and removal w/ HexData wrapper
func add_hex(hex, data):
func move_hex(hex_old, hex_new):
func remove_hex(hex):
func get_hex(hex):
func get_all_hex():
func get_wall(hex, direction):

Rotation Transforms
func rotate_hex_left(hex):
func rotate_hex_right(hex):

Pixel func and things useful to drawing.
func hex_to_pixel(hex):
func pixel_to_hex(pos):
func round_hex(hex):
func hex_corner_offset(corner):
func hex_corners(hex):

Return the coordinates of a direction from a given hex
func neighbor_hex(hex, direction):
func diagonal_neighbor_hex(hex, direction):

Distance and from origin hex lengths.
func hex_length(hex):
func hex_distance(hex_a, hex_b):
```
