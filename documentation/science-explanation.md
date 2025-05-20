# The Science of Acoustic Levitation

Acoustic levitation might seem like magic, but it's based on well-established principles of physics. This document explains the scientific principles that make our acoustic levitator work.

## Basic Principles

Acoustic levitation uses sound waves to exert pressure on objects, counteracting the force of gravity and allowing objects to float in mid-air. This is possible because sound waves, like all waves, carry energy and momentum.

## Standing Waves

The key to acoustic levitation is the creation of standing waves. A standing wave occurs when two waves of the same frequency travel in opposite directions and interfere with each other.

In our levitator, we create standing waves by:
1. Generating sound waves from the top array of transmitters
2. Generating sound waves from the bottom array, 180° out of phase with the top
3. The waves interfere, creating a pattern of nodes (where the waves cancel out) and antinodes (where they reinforce)

![Standing Wave Diagram](../media/photos/standing_wave.jpg)

## Acoustic Radiation Pressure

When sound waves interact with an object, they exert a small force called acoustic radiation pressure. This occurs because the sound waves transfer momentum to the object.

At certain positions in a standing wave (specifically at the pressure nodes), the acoustic radiation force can balance the gravitational force acting on small objects, causing them to levitate.

## Mathematical Description

The acoustic radiation force (F) on a small spherical object in a standing wave can be approximated by:

F = (π × P²× V × k × sin(2kz)) / (2 × ρ × c²)

Where:
- P is the acoustic pressure amplitude
- V is the volume of the particle
- k is the wave number (k = 2π/λ, where λ is wavelength)
- z is the position along the axis of the standing wave
- ρ is the density of the medium (air)
- c is the speed of sound in the medium

For levitation to occur, this force must equal the gravitational force:

F = m × g

Where:
- m is the mass of the object
- g is the acceleration due to gravity (9.81 m/s²)

## Wavelength and Node Spacing

For our 40kHz ultrasonic transmitters, the wavelength (λ) is:

λ = c / f = 343 m/s ÷ 40,000 Hz = 8.575 mm

In a standing wave, the pressure nodes (where objects can levitate) are spaced at intervals of λ/2 = 4.29 mm.

## Size Limitations

The maximum size of an object that can be levitated depends on:
1. The wavelength of sound used (smaller wavelengths can only levitate smaller objects)
2. The acoustic power provided by the transmitters
3. The density of the object

Generally, objects smaller than λ/2 can be levitated more easily, which is why our 40kHz system works well for objects up to about 3-5mm in size.

## Multi-Axis Levitation

While our basic design uses a single axis (vertical), more advanced systems can use three perpendicular axes to create a more stable "acoustic trap" that can hold objects more securely.

## References

1. Brandt, E. H. (1989). Levitation in Physics. Science, 243(4889), 349-355.
2. Xie, W. J., & Wei, B. (2007). Parametric study of single-axis acoustic levitation. Applied Physics Letters, 90(20), 204104.
3. Marzo, A., Seah, S. A., Drinkwater, B. W., Sahoo, D. R., Long, B., & Subramanian, S. (2015). Holographic acoustic elements for manipulation of levitated objects. Nature Communications, 6(1), 1-7.
4. Foresti, D., Nabavi, M., Klingauf, M., Ferrari, A., & Poulikakos, D. (2013). Acoustophoretic contactless transport and handling of matter in air. Proceedings of the National Academy of Sciences, 110(31), 12549-12554.
5. Andrade, M. A. B., Pérez, N., & Adamowski, J. C. (2018). Review of Progress in Acoustic Levitation. Brazilian Journal of Physics, 48(2), 190-213.
