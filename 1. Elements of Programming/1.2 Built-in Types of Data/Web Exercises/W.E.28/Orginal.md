**Barycenter.** In a two-body system, the [barycenter](https://en.wikipedia.org/wiki/Barycenter) is the center of gravity about which the two celestial bodies orbit each other. Given the masses m1 and m2 of two bodies, and the shortest distance a between the two bodies, write a program to compute the distance from the center of the first (more massive) body to the barycenter: r1 = a m2 / (m1 + m2).
Here are a few examples. Masses are in earth-mass units, distances are in kilometers.

Earth-moon: m1 = 1, m2 = .0123, a = 384,000, r1 = 4,670, R1 = 6,380.

Pluto-Charon: m1 = .0021, m2 = .000254, a = 19,600, r1 = 2,110, R1 = 1,150.

Sun-Earth: m1 = 333,000, m2 = 1, a = 150,000,000, r1 = 449, R1 = 696,000.

Note that if r1 is less than the radius of the first body R1, then the barycenter lies within the first body.
