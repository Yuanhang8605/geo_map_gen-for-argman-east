# geo_map_gen-for-argman-east
use cython to rewrite the geo_map part of https://github.com/argman/EAST
to build the lib, in the geo_map_cython_lib directory, run "sh build_ext.sh"

to use the lib, in the icdar.py file add:
```python
from geo_map_cython_lib import gen_geo_map

# in the icdar.py, delete the 570~582 lines, replace the code with:
gen_geo_map.gen_geo_map(geo_map, xy_in_poly, rectangle, rotate_angle)
```


