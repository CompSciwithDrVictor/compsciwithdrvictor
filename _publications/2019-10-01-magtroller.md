---
title: "Tangible Around-Device Interaction Using Rotatory Gestures with a Magnetic Ring"
collection: publications
category: conferences
permalink: /publications/2019-10-01-magtroller
excerpt: 'This paper explored the mobile gameplay context by implementing an interface that uses rotatory gestures from a magnetic ring as input, and compared with some other typical ways of input.'
date: 2019-03-17
venue: 'Human-Computer Interaction with Mobile Devices and Services'
paperurl: '../files/publications/2019/Tangible_Around-Device_Interaction-MobileHCI2019.pdf'
citation: 'V. Cheung and A. Girouard. 2019. "Tangible Around-Device Interaction Using Rotatory Gestures with a Magnetic Ring". In Proceedings of the 21st International Conference on Human-Computer Interaction with Mobile Devices and Services (MobileHCI''19). ACMachinery, New York, NY, USA, Article 26, 1–8. https://doi.org/10.1145/3338286.3340137'
---

<!--
![an image of the device setup](/images/2019-10-01_magtroller_thumbnail.jpg)
-->

<iframe width="560" height="315" src="https://www.youtube.com/embed/oGJstblyvII?si=g04BVdCi5KTiDbhx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Abstract
------
The majority of mobile applications use built-in touchscreens and/or accelerometers to provide direct ways for user inputs. Yet, the need to manipulate the device itself (e.g. touch, tilt) poses usability issues such as occlusion and inaccuracy. To address these issues, research proposed using the built-in magnetometer and magnets to facilitate around-device interactions. However, there is little evaluation in how this technique impacts performance and user experience beyond simple docking tasks. To fill this gap, we explored the mobile gameplay context by implementing an interface that uses rotatory gestures from a magnetic ring as input, and compared two control mappings (angular and linear) with touch and tilt in a usability study using a mobile game. We found that rotatory gestures with the ring, when mapped to angular controls, were on par with touch and superior over tilt, and engendered greater gameplay experience and sense of mapping. Based on our findings, we discuss implications of using this technique for gameplay, as well as other applications.

Reflection
------
This project is based on a small idea I had when playing with a magnetic ring -- a magic prop. I knew that every modern mobile device has a magnetometer to measure the magnet field around it, mostly for the map application to determine where North is. What I didn't know was how easy it was to capture that data and map them to the degree of rotation.

Applying that information one can control almost anything that uses a numerical value (e.g., volume, brightness). As a demonstration, we mapped it to a game controller, and did some comparative studies with other typical input methods (touch and tilt).

I think making use of external objects to control things on a mobile device is very promising because it addresses the occulsion problem of touchscreen devices, while enjoying the benefits of tangible user interactions.