# expose-private-data
Make use of graphical glitches to exploit sensitive data from other tabs and apps. Works in browsers based on Chromium.

The glitch is only present on certain devices. See (list) for devices found vulnerable.

## Exploiting the glitch:
1.	 Open Chrome.
2.	 Visit https://zznidar.github.io/expose-private-data/www/ (open a few other tabs as well).
3.	 During the first 40 ticks (a few seconds, depending on the device speed), the website will take canvas snapshots with javascript. During this time, switch between tabs and between applications (switch and go back to this tab).
4.	 After 40 ticks, 40 buttons will appear. Press each of them to download the corresponding snapshot (I tried to automate this, but Chrome didn’t allow the site to automatically download 40 files).
5.	 Look at the snapshots. Parts of recently rendered graphics will appear on certain snapshots.


The left number always shows the current tick. On the right, you can see the numbers of ticks when the website was resumed (i. e. when you changed back to that tab).

According to my tests, the glitches always appear on snapshots 2 and 3 ticks after the site is resumed. Sometimes parts of them are just transparent, other times they contain recently rendered data.
