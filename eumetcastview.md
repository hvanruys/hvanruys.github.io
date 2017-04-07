---
layout: page
title: EUMETCastView introduction
---


When you launch EUMETCastView, you should get a screen that looks like this:

![_config.yml](/images/Screenshot_eumetcastview_ephem.jpg)

The screen is divided in three parts :

- the dockable toolbar ( can be moved left, right, up and down)
- the Toolbox
- the selected page

The toolbar allows you to select the different pages. At startup, the program will show the 'Satellite Setup Page'.

## The Satellite Setup Page

The satellite setup page allows you to setup the different segment directories, selecting the date of segments to load and selecting the satellites in the Two Line Elements list.

The widget 'List of segment directories' displays the target directories

Satellite's are selected in the 'TLE Files' widget. These selected satellites are displayed in the 'Cylindrical Equidistant' page and the '3D Globe' page.

In the 'Segment directories' widget you can select which directories you want to load. By selecting a date in the calendar widget all the image segments <ins>information</ins> *(not the image data itself)* of all the selected directories are loaded in the program. This is used for displaying the positions of the image segments in the 'Cylindrical Equidistant' page and '3D Globe' page.

## The Geostationary satellite page

After loading the satellite segments information, an overview of the segments are displayed per satellite. The following geostationary satellites are available in <strong>EUMETCastView</strong> :

- Meteosat 10
- Meteosat 9
- Meteosat 7
- FengYun 2E
- FengYun 2G
- GOES 13
- GOES 15
- MTSAT2

For GOES-13, GOES-15 and MTSAT2 there are segments transmitted in 'Data Channel 3' and 'Data Channel 4'. Those segments are displayed in different tabs.

By clicking on an entry in one of the tabs you select the image by date and time to compile. The required channel is selected in the Toolbox.

![_config.yml](/images/Screenshot_eumetcastview_geostationary.jpg)

## The Cylindrical Equidistant page

In this page all the <strong>real time</strong> positions of the selected satellites are visible. At the bottom of the page you can select which segment tracks you want to see. The following polar satellite segment tracks are possible

- Metop segment tracks (Metop-A and Metop-B)
- Noaa segment tracks ( from NOAA-19)
- HRP segment tracks (the Metop-A and Metop-B segment tracks via the EARS service)
- GAC segment tracks (low resolution NOAA-19 images)

To make a combined picture of the segments you right-click on the start of the segments ( yellow points along the red segment tracks ) to select them. The button 'Make Image' will render a combined satellite image. By moving the vertical scroll bar, the segment tracks will move over the cylindrical equidistant picture.
A more straightforward method for selecting segments is possible in the '3D Globe' page.

![_config.yml](/images/Screenshot_eumetcastview_cylindrical.jpg)


## The 3D Globe page

The 3D globe makes it easier to select the segments of interest. By right clicking <strong>in</strong> the boundery of the segment you can select or deselect this segment. By moving the vertical scroll bar on the right of the 3D globe, the segment tracks will move over the globe in function of time. Again, the button 'Make Image' will render the satellite image in the image page. When the button 'Texture on' in the toolbox page is set, the image will also be rendered to the texture of the 3D globe. You can toggle this button from 'Texture On' to 'Texture Off'.

![_config.yml](/images/Screenshot_eumetcastview_globe.jpg)

## The image page

After rendering the image you can view it in the Image page.

![_config.yml](/images/Screenshot_eumetcastview_image.jpg)

## The Toolbox page

The Toolbox allows you to select which image you want to render.

<h5 class="text_line">The AVHRR tab</h5>

<img src="/images/Screenshot_toolbox_avhrr.jpg" alt="avhrr toolbox" class="TextWrapLeft">

All the five channels of the AVHRR image are compiled at the same time. By clicking the channel button the chosen channel will be displayed. The color image is assembled when the image is compiled.

<h5 class="text_line">The VIIRS tab</h5>
<img src="/images/Screenshot_toolbox_viirs.jpg" alt="viirs toolbox" class="TextWrapRight">

The selecting of the channels for VIIRS images is done in the VIIRS tab. By clicking on the button 'Show VIIRS image' the selected channel will be rendered.

<h5 class="text_line">The Geostationary tab</h5>
<img src="/images/Screenshot_toolbox_geostationary.jpg" alt="geostationary toolbox" class="TextWrapLeft">

For geostationary images the available channel buttons will be enabled depending on the chosen geostationary satellite image.

<h5 class="text_line">The Projections tab</h5>
<img src="/images/Screenshot_toolbox_projections.jpg" alt="projections toolbox" class="TextWrapRight">

When an image is rendered ( AVHRR, VIIRS or geostationary ) it is possible to render a projection of this image. The following projections are possible :

- the Lambert Conformal Conic projection
- the General Vertical projection
- the Stereographic projection
