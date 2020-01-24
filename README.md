#### Table of contents:

- [Quick pills](#quick-pills)
- [Rossby number](#rossby-number)

# Quick pills
* A strictly convex domain is one that is possible to bound from below with a quadratic thing.
* A strictly matrix that is row/column diagonally dominant is non singular.
* The laplacian is "null" at point of "equilibrium". Thinking in terms of the heat equation, it is positive at points where temperature is low, meaning that temperature as a fluid will tend to flow towards those spots; and it is negative at points of high temperature, as temperature will tend to flow away from them. Another nice interpretation: \Delta f(0) measures average difference f(x)-f(0) over small balls around 0 (see https://math.stackexchange.com/questions/50274/intuitive-interpretation-of-the-laplacian).

# Rossby number
To describe whether a phenomenon is *large-scale*, i.e. if it is affected by earth's rotation. How to quantify if a flow is affected by earth's rotation?

Consider two quantities `L` and `U`, with `L` being a characteristic scale-length of the phenomenon (ex. distance between two peaks, distance between two isobars) and `U` the horizontal velocity scale of the motion. The ratio `L/U` is the time it takes to the motion to cover a distance `L` with velocity `U`. If this time is bigger than the period of earth's rotation, then the phenomenon IS affected by the rotation. 

So if `L/U \geq 1/\Omega`, the phenomenon IS a *large-scale* one. Thus we can define `\epsilon = U/2L\omega` and say that for `\epsilon \leq 1` a phenomenon is large scale. Phenomena with small Rossby number are dominated by Coriolis force behavior, while those with large Rossby number are dominated by inertial forces (ex: a tornado). However, rotational effects are more evident for low latitudes (i.e. near the equator), so the Rossby number can be different depending on where on earth we are.

(Notice that `\Omega` is in theory equal to `2\omega\sin(\phi)`, with \omega being the earth rotational velocity and \phi the angle between the axis of rotation and the direction of fluid movement. In the geophysical context, flows are mostly horizontal (also due to density stratification in both atmosphere and ocean), so `\sin(\phi)` collapses to 1. There is a bunch of different notation, but this `\Omega` is also referred to as `f`, called the *Coriolis frequency*)
