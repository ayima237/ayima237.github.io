---
layout: post
title: Planet Volumes
image: "![image](https://github.com/user-attachments/assets/b331a94e-a1c7-4bc3-855a-63b5b337aeab)
"
tags: [Python, Planets]
---

# This project
## is all about
### how Python can
#### Calculate the volume of
##### a million imaginary Planets
###### via in a very short time period!

---

First, I will import the numpy functionality which is what we will be using for our calculation.

```
import numpy as np

```

A quick research online gave the radii of planets as seen above which we will assign to the variable radii!
Mercury: 2439.7 km
Venus: 6051.8 km
Earth: 6371.0 km
Mars: 3389.5 km
Jupiter: 69911.0 km
Saturn: 58232.0 km
Uranus: 25362.0 km
Neptune: 24622.0 km

```
radii = np.array([2439.7, 6051.8, 6371.0, 3389.5, 69911.0, 58232.0, 25362.0, 24622.0])

```

Remember in maths volume(area) of a sphere = 4/3 * pi * r**3
So, using the np.pi functionality, volume of the first planet will be calculated as;

```
r = 2439.7
volume = 4/3 * np.pi * r**3
print(volume)

```
Remember that we created a one dimensional array of radii for all 8 planets above. Now, I will use that to calculate the volume of all eight planets simultanously.

```
volumes = 4/3 * np.pi * radii**3
print(volumes)

```
Now, Imagine having to calculate the volume of 1 million imaginary planets on python simultaneously. I will use the randon=m functionality to create 1 million random integers between 1 and 1000 which I will be using as the redii for this purpose. See in the below code.

```
redii = np.random.randint(1, 1000, 1000000)
print(radii)
volumes = 4/3 * np.pi * radii**3
print(volumes)

np.sort(volumes)

```
Here is an _ordered list_ showing the volumes of our 1 million imaginary planets in ascending order.


![alt text](https://github.com/user-attachments/assets/5935477b-4838-4f45-bd22-367336733b44)
!")
