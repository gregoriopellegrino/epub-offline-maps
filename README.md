#epub-offline-maps

An EPUB widget to display offline maps with geolocation and POIs

## Project
The idea is to make available interactive offline maps in EPUBs for making travel guides and other publications.  
Since it isn't possible to embed an online map into an EPUB (like Google Maps), I looked for a solution to make it available offline.  
Offline maps are perfects because they work also when you are abroad and you don't have an internet connection.  

## How I did
I looked for a solution for offline maps on mobile devices and I found this article: http://davidrs.com/wp/phonegap-3-0-leaflet-offline-maps/  
Then I used Mobile Atlas Creator (http://mobac.sourceforge.net/) for downloading the tiles of the region I was interested: Turin (my town) in Italy.  
I downloaded the JavaScript library Leaflet (http://leafletjs.com/)  
I packaged all in an EPUB3 file *et voilat*, it works!

## Test
The project has been tested on:
- Adobe Digital Editions 4.0 (on OS X Yosemite): **OK**
- iBooks 1.1 (on OS X Yosemite): **doesn't work**
- iBooks 3.2 (on iOS 7.0.6): **doesn't work**
- Readium (on Chrome): **OK**

## Todo
- add the geolocation (http://leafletjs.com/reference.html#map-locate)
- add POIs
- test on Readium SDK (Kobo, ecc.)
- pack it as an EPUB widget (http://www.idpf.org/epub/widgets/)

## License
© 2014 Gregorio Pellegrino
All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are
permitted provided that the following conditions are met:

   1. Redistributions of source code must retain the above copyright notice, this list of
      conditions and the following disclaimer.

   2. Redistributions in binary form must reproduce the above copyright notice, this list
      of conditions and the following disclaimer in the documentation and/or other materials
      provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY
EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR
TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.