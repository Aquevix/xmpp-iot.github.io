---
layout: archive
title: "Gsoc 2016"
date: 2015-03-001T09:44:20-04:00
modified:
categories: 
excerpt: "XMPP-IoT is part of Google summer of code 2016"
image:
  feature: 
  teaser: prototyping-iot_400x250.png
  thumb: prototyping-iot_400x250.png
share: true
ads: false
---
***Interoperability  testtool for IoT*** is a project within XMPP that is part of the [google summer of code 2016](https://developers.google.com/open-source/gsoc/) This years XMPP-IoT project will focus on creating an interoperabilty testing environment for XMPP based distributed devices pretty much the same idea as on http://xmpp.net. You will add a JID to testtool and it will perform a number of Interoperabilty tests to se what capabilities the device has.

getting started:

# Teaser tasks for 2016
Below you find the teaser tasks for 2016 
Mentor for the projekt is [Joachim Lindborg](http://lsys.se) and is reachable at

  -xmpp:jabberjocke@jabber.se 

  -twitter:@joachimlindborg
  
  * teaser tasks should be tested and ran on your own environment before sen in with pullrequest 
  * Change this page with a pullrequest when you have done a tesertask so others can focus on the other ones
  * Keep Joachim Lindborg in the loop when you choose a task
  * Feel free to come with your own suggestions of a teaser task *encouraged*

## Getting started
Go through this site and and of course http://xmpp.org/ to get the idea of what Internet of Things is and how XMPP is a good fit for that. Then look at the Tutorials and the documentation on SleekXMPP. A good thing to go further is also to look at the extensions especially xep323 and xep325

  * http://xmpp.org/
  * http://xmpp.org/uses/internet-of-things.html
  * http://www.xmpp-iot.org/tutorials/python-tutorial/
  * http://sleekxmpp.readthedocs.org/en/latest/
  * http://xmpp.org/extensions/
  * http://xmpp.org/extensions/xep-0323.html
  * http://xmpp.org/extensions/xep-0325.html

## 1. Logging data in a database
One of the crucial things in IoT is storing data you should extend the [History logger script](https://github.com/joachimlindborg/SleekXMPP/tree/xep_0323_325/examples/IoT) with possibilty to store the data in a database either locally or on a remote system. Do the work in a plugin fashion so it will be easy to extend with other database api's in the future. Also create a tutorial on this site to show how it works. ex database could be https://influxdata.com/

  [ ]**Done by:**

## 2. XMPP-IoT'ifying a device
in the [example catalog](https://github.com/joachimlindborg/SleekXMPP/tree/xep_0323_325/examples/IoT) you find an example on extending the PhilipsHue gateway so it can be used over the XMPP-IoT network. Find another API based IoT device or system and extend it so it can be accessed over the XMPP network. some ideas:

  [ ]http://developer.xively.com/ **Done by:**

  [ ]https://dev.netatmo.com/doc **Done by:**

  [ ]Add your own thing **Done by:**

## 3. Make a script querying another devcie's capabilities
[XEP 0030 Disco](http://xmpp.org/extensions/xep-0030.html) is a way in XMPP to discover another XMPP enpoint's capabiilties. Create a script in the [example catalog](https://github.com/joachimlindborg/SleekXMPP/tree/xep_0323_325/examples/IoT) catalog that query another JID for it capabilities and list's the IoT realted Xep's it supports in a nice fashion prefrably creating a nice markdown page. 

  [ ]**Done by:**

# Last year Google summer of code 2015
Last years project is kept here as a reference [google summer of code 2015](http://www.google-melange.com/gsoc/homepage/google/gsoc2015). The project created a gui and a cordova application that you can use for this summers work.

Deliverables
  * IoT Protocols implementation for XMPP Chat Client Converse.Js
  * Cross Platform Mobile Application for Sensoring and Controlling of Data sent or received by Devices
  * History Logger for Sensor Devices

<div class="tiles">
{% for post in site.categories.gsoc %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
