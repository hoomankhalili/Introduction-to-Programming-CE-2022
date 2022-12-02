**Equatorial to horizontal coordinates.** The equatorial coordinate system is widely used by astronomers to indicate the position of a star on the celestial sphere. The position is specified by its declination δ, its hour angle H, and its latitude φ. The horizontal coordinate system (a.k.a. Alt/Az coordinate system) is useful for determining the setting/rising time of celestial objects. The position is specified by its altitude (vertical angle from the horizon) and and its azimuth (horizontal angle). Given a star's position using equatorial coordinates, find its position in horizontal coordinates using the formulas below:
````
Altitude = asin (sin φ sin δ  + cos φ cos δ cos H)
Azimuth  = acos ((cos φ sin δ  - sin φ cos δ cos H) / cos (Altitude) )
````
