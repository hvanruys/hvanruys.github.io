---
layout: post
title: New release v1.1.2
---

Changes made in EUMETCastView v1.1.2 :

- Added a Configuration database for VIIRS M.
- The VIIRS M and VIIRS DNB images have there own image memory, and so it is possible to view the two images together.
- Change of the Projection tab to include the new input image.
- New radiobutton in the Projection tab that allows to combine the VIIRS M and VIIRS DNB images.
- Moved the track buttons vertical to the right and included an overview counter of the selected segments.


**How to use the radiobutton "Combine with background"**

 - In the 3D Globe window select the segments over the area of interest for the VIIRS M band.
 - Make the VIIRS M image. Because the DNB segments are always at night, choose for example Blue for M13, Green for M14 and Red for M15.
 - Select the VIIRS DNB segements over the same area.
 - Make the VIIRS DNB image. 
 - Go to the 'Image' window. You can view the two images by clicking on the 'M-Band' tab or the 'Day/Night Band' tab.
 - Select the 'Projection' tab, choose the kind of projection and select the projection area of interest.
 - Select the 'Input Images' radiobutton 'VIIRS M Image' and create the projection map.
 - Select the 'Input Images' radiobutton 'VIIRS DNB Image' and also select the 'Combine with background' radiobutton. The background (the VIIRS M image) will be combined with the VIIRS DNB Image.

![_config.yml](/images/spaincombine.jpg)

Download it at <a href="https://github.com/hvanruys/EUMETCastView/releases">Github</a>.
