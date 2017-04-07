---
layout: post
title: New release v1.2.4
---

In release v1.2.4 the download of OLCI EFR/ERR and SLSTR segments from Scihub or CODA is integrated in EUMETCastView.

The first thing to do is entering your userid and password for the Scihub or CODA website in 'Set Preferences' - 'Scihub/CODA Config' window. Choose your data provider and indicate in which kind of image your interested. The Scihub/CODA websites contains all the OLCI EFR/ERR and SLSTR segments. The downloaded products are saved in the 'Product Directory'.

- The Preferences window for Scihub/CODA Config.

![_config.yml](/images/Screenshot_Preferences_Scihub.jpg)


For downloading the **available** segments, choose the date in the calendar, go to the 3D Globe and push the 'Download available segments from Scihub/CODA' button. An XML file will be created, and you can see the progress of the download on the 3D-Globe window. Once the download is complete, all the **available** segments are displayed on the 3D-Globe. 

![_config.yml](/images/Screenshot_3DGlobe_SLSTR.jpg)

To download the required products, select the segments on the 3D Globe. The selected segments will appear in the list 'Products selected for download'. The total number of bytes to download is given underneath the list.
To start the download push the 'Start Download products' button. Scihub and CODA only allows 2 simultaneous downloads. The status in the list goes from 'waiting' to 'Busy (downloading)' and finaly 'Finished' when the download is complete.

![_config.yml](/images/Screenshot_download_product.jpg)

To process the downloaded segments, you have to include the 'Product directory' in the 'List of segment directories' of the 'Satellite Setup' window. The downloaded segments will appear on the 3D Globe where they can be processed as segments coming from Eumetcast.

When starting up EUMETCastView, the program will allways try to find an XML file with **available** segments for the current day. If the file is not found or the segments are from another date then the current day, nothing is displayed on the 3D Globe. 

Download it at <a href="https://github.com/hvanruys/EUMETCastView/releases">Github</a>.
