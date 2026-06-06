# XMIT - New tools for old jobs

This repository has design files and (soon) code for a direct synthesis digital 
mode transmitter optimized for use on amateur bands. It should work well up to 
2m. The novelty here relative to other systems like the [QDX](https://qrp-labs.com/qdx.html)
lies in a few areas:

a) the use of [74LVC2G157](https://www.ti.com/lit/ds/symlink/sn74lvc2g157.pdf) to generate differential drive for a differential
driver such as the [THS6232](https://www.ti.com/lit/ds/symlink/ths6232.pdf) which can
directly drive most balanced antennas without a balun at up to about 5W. This design
avoids the need for fancy gate drive or paralleling FETs in favor of SMT packaging everywhere. 

b) the use of SMT inductors and SMT analog switches such as the 
[74lvc2g53](https://www.ti.com/lit/ds/symlink/sn74lvc2g53.pdf) or 
[74lvc1g66](https://www.ti.com/lit/ds/symlink/sn74lvc1g66.pdf).
This change is not earth-shattering, but it allows a much tighter all-SMT design with as much as 80dB suppression of harmonics.
The high degree of suppression is achieved by using a filter tuned to put the response zeros directly on the harmonics
and careful filter layout to suppress parasitic coupling.
