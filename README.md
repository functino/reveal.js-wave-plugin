Advance through your [reveal.js](https://github.com/hakimel/reveal.js) presentation slides by waving 
=====================================

This plugin for [reveal.js](https://github.com/hakimel/reveal.js) makes it possible to use your webcam to detect waving - and then triggering a slide change.
It's more of a cool effect than a useful/productive plugin - but great to impress your audience.

You can see a live demo of it here: http://functino.github.com/reveal.js-wave-plugin/

Restrictions
=======
- works only in Chrome (only Chrome supports getUserMedia() which is used to get access to your webcam)
- it only works if your calling the presentation on a server (i.e not with a file:// url)
- you must accept Chrome's request to use your webcam
- at the moment only going forward in your presentation is enabled


HowTo / Installation
=======
Just copy this repository into your reveal.js presentation to `/plugin/wave`.

Include this two lines in the "dependencies" section in index.html:
`{ src: 'plugin/wave/webcam-swiper-0.1.js'},
{ src: 'plugin/wave/client.js'}´

Run the server.js file via node to startup a server on localhost:1947 (or use any other server to serve the presentation, for example the speakernote plugin has it's own server wich will do just fine). If you use my server.js be sure to install the needed modules - for example with a simple `npm install -d`.
Open the presentation, click "accept" when Chrome asks you to grant permission to use the webcam and then wave/swipe in front of your webcam  to advnace through your slides.


Thanks
=======
The webcam-swiper library is from https://github.com/iambrandonn/WebcamSwiper