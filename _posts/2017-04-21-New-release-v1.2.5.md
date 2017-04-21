---
layout: post
title: New release v1.2.5
---

In release v1.2.4 it was already possible to save OLCI EFR/ERR segments as a 48bit RGB PNG image. In this release you can save the projection image (for the Lambert, the vertical and the Stereographic projection) for the OLCI EFR/ERR and VIIRS M as a 64bit RGBA PNG image. The internal calculations for the projected image are done with the maximum precision of 12 bits, because the bit depth of the OLCI and VIIRS sensor are 12 bits. If the projected image contains pixels that where not valid or the segments didn't cover the complete projected image, the Alpha value of such pixels are zero. Image processing software (like Gimp 2.9.5 or Photoshop) can use this feature to process the image. A radiobutton 'mapped to 0 - 65535' multiplies every pixel value by 16. 

Download it at <a href="https://github.com/hvanruys/EUMETCastView/releases">Github</a>.
