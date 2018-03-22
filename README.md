# Minutiae Detection using Crossing Number Method

Crossing number methods is a really simple way to detect ridge endings and ridge bifurcations.

First, you'll need thinned (skeleton) image. Then the crossing number algorithm will look at 3x3 pixel blocks:
* if middle pixel is black (represents ridge):
    * if pixel on boundary are crossed with the ridge once, then we've found ridge ending
    * if pixel on boundary are crossed with the ridge three times, then we've found ridge bifurcation
