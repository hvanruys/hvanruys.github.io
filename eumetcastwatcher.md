---
layout: page
title: EUMETCastWatcher
---

The Tellicast program receives the EUMETCast files and they are written to a target directory that is defined in **recv-channels.ini**. For example :

<div class="message">
[EUMETSAT Data Channel 1]<br>
target_directory=\media\VOL2T\received\Data Channel 1<br>
[EUMETSAT Data Channel 2]<br>
target_directory=\media\VOL2T\received\Data Channel 2<br>
[EUMETSAT Data Channel 3]<br>
target_directory=\media\VOL2T\received\Data Channel 3<br>
[EUMETSAT Data Channel 4]<br>
target_directory=\media\VOL2T\received\Data Channel 4<br>
...<br>
</div>

<strong>EUMETCastWatcher</strong> performes two things: first it will delete the files in which we are not interested and secondly, to manage the large amount of files, EUMETCastWatcher will create a subdirectory under the target directory for every new day and moves the received files to that subdirectory.
This new subdirectory will have the layout YYYYMMDD.
For example :

<div class="message">
\media\VOL2T\received\Data Channel 1\20141205<br>
\media\VOL2T\received\Data Channel 1\20141206<br>
\media\VOL2T\received\Data Channel 1\20141207<br>
\media\VOL2T\received\Data Channel 1\20141208<br>
\media\VOL2T\received\Data Channel 1\20141209<br>
...
</div>

In the setup dialog of the program you must indicate which directories to monitor. Directories which are not in that list will receive the files in the target directory and will not be deleted or moved to the subdirectory.

By comparing the received filenames with a file template the program is able to delete or move the file to the desired subdirectory.

![_config.yml](/images/Screenshot_eumetcastwatcher.jpg)

An example of the ini file:

<div class="message">
[segments]<br>
<p>filetemplatelist=avhrr_*_noaa19.hrp.bz2, AVHR_HRP_00_M01_*.bz2, AVHR_HRP_00_M02_*.bz2, AVHR_xxx_1B_M02_*, AVHR_GAC_1B_N19_*, L-000-MSG1*, L-000-MTP___-MET7*, L-000-MSG3__-GOES15*, L-000-MSG3__-GOES13*, L-000-MSG3__-GOES15*, L-000-MSG3__-MTSAT2*, AVHR_xxx_1B_M01_*, H-000-*, SVMC_npp_d*</p>
<p>segmentdirectories=/media/Vol2T/received/Data Channel 1, /media/Vol2T/received/EPS-15, /media/Vol2T/received/Data Channel 2, /media/Vol2T/received/Data Channel 6, /media/Vol2T/received/Data Channel 3, /media/Vol2T/received/Data Channel 5, /media/Vol2T/received/Data Channel 4, /media/Vol2T/received/EPS-10, /media/Vol2T/received/NPP-2</p>
<p>startdatetemplatelist=6, 16, 16, 16, 16, 46, 46, 46, 46, 46, 46, 16, 46, 10</p>
</div>
