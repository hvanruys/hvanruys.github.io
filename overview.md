---
layout: page
title : Overview
---

The Open Source program **EUMETCastView** allows you to view and manipulate

- AVHRR images from NOAA-19, Metop-A and Metop-B.
- VIIRS images from SUOMI-NPP.
- OLCI EFR and ERR images from Sentinel-3A
- and HRIT/LRIT images from Meteosat-10, Meteosat-9, Meteosat-8, Electro L2, FengYun 2E, FengYun 2G, GOES-15, GOES-16 and Himawari-8.
 
Examples of images received with EUMETCastView can be found on the <a href="https://www.flickr.com/photos/137270544@N02/">flicr</a> website.

After creating the image you can use 3 kinds of projections for redisplaying the image

- the Lambert Conformal Conic projection
- the General Vertical projection
- the Stereographic projection

<div class="message">
More detailed information about EUMETCast can be obtained from <a href="http://www.eumetsat.int/website/home/Data/DataDelivery/EUMETCast/index.html">this page</a> and <a href="http://www.eumetsat.int/website/wcm/idc/idcplg?IdcService=GET_FILE&dDocName=PDF_TD15_EUMETCAST&RevisionSelectionMethod=LatestReleased&Rendition=Web">TD 15: EUMETCast — Broadcast System for Environmental Data (PDF, 3 MB)</a>. Also there are the excellent webpages of <a href= "http://www.satsignal.eu/">David Taylor</a> with a good description of the <a href="http://www.satsignal.eu/wxsat/atovs/index.html">hardware</a> needed. There is also <a href="http://www.geo-web.org.uk/">The Independent Organisation for Weather Satellite and Earth Observation Enthusiasts</a>.
</div>

The following webpages describes the software needed for a station setup with 2 PC's; one for receiving the EUMETCast transmissions and one for viewing and manipulating the received images.
The receiver PC runs the following software

- the **TelliCast** software (tc-recv)
- **EUMETCastWatcher** ( a simple monitoring program )

The PC for viewing and manipulating the images runs the **EUMETCastView** software.

**System requirements**

The programs are written in C++ with Qt 5.5 and it is possible to compile them for both Windows and Linux.
The receiver system (where the **Tellicast** and **EUMETCastWatcher** software is installed) can be a modern 32 or 64 bit Linux or Windows PC, but the system that runs **EUMETCastView** definitely needs a 64 bit system with a minimum of 6 GByte of RAM. For OLCI images 12 GByte RAM is needed.

**Shoreline database**

**EUMETCastView** uses a  <a href="http://www.soest.hawaii.edu/pwessel/gshhg/">geographic database</a> for the coastline overlays that is displayed in the 3D Globe and the various projections. You need to download the **native binary files** of the database from <a href="http://www.soest.hawaii.edu/pwessel/gshhg/gshhg-bin-2.3.4.zip">here</a>.

**Software dependencies**

The program uses the <a href="https://www.hdfgroup.org/HDF5/release/obtain5.html">HDF5</a> and <a href="http://www.unidata.ucar.edu/software/netcdf/">netCDF</a> libraries for decoding the images. The necessary dll's are included in the zip file that you can download from <a href="https://github.com/hvanruys/EUMETCastView/releases">github</a>.
A working OpenGL (>= 3.2) environment is also required.

