# HD6309 SBC Backplane

This projects defines a backplane expansion system
for the HD6309 Single Board Computer I designed 
(see https://github.com/jimbro1000/HD6309sbc)

Each backplane panel provides two slots for the 
100mm x 100mm expansion tiles plus a pair of 
"sideways" connector to add extra backplane panels 
to either side.

Hypothetically you could keep expanding but in 
real terms the drivers on each chip can only 
connect to a limit number of other chips, this
places real term limits of 4 - 6 tiles without
buffering, especially on the address and data
lines

## Tile layout

The positioning of connectors for the tiles is
defined by the layout of the main SBC tile, as
such it is essential that the relative position
of the two power and expansion connector of each
tile is maintained

### Alternative layouts

Provided the relative tile connector positions are 
maintained the layout of boards does not need to
be two dimensional.

## Power input

All of the tiles (so far) require +5V and ground.
It is expected that the primary tile provides the
power input from an external source, with good
regulation of power and current. Adding extra
tiles may place unexpected load and cause drop
outs or unpredictable behaviours