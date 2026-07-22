# SCANS Survey

These Github pages include software and instructions for running an advanced visual data collection system, primarily targetted at ship based visual line transect surveys for cetaceans.

The work builds on a system created by Doug Gillespie and Russell Leaper for the 2005 SCANS II survey [An Integrated Data Collection System for Line Transect Surveys](https://doi.org/10.47536/jcrm.v11i3.601) 

The newest iteration of the system brings in two important changes:

1. We now use [forms](https://www.pamguard.org/olhelp/visual_methods/loggerFormsHelp/docs/loggerFormsOverview.html) inside the [PAMGuard](www.pamguard.org) software instead of the out of date and unsupported [Logger 2000 software](https://www.marineconservationresearch.co.uk/downloads/logger-2000-rainbowclick-software-downloads/).
2. All of the wired buttons, webcams, microphones, etc. used by each observer have been replaced with a mobile phone app.

This means that (we hope) all components required to use this system can be bought off the shelf without any need to build and maintain bespoke hardware.  

This is a work in progress, targetting surveys in the summer of 2027, hopefully with testing at sea earlier that year, or possibly late 2026. 

This GitHub organisation will contain repositories of software developments specific to this survey method and also repositories of important configuration files and sample databases that you'll probably want to help get a system up and running. 

The main code development repositories are currently:

1. [scansapp](https://github.com/SCANS-Survey/scansapp) - an Android (phone or tablet) app that has sightings buttons, captures webcam images, and sends voice to the PAMGuard data recorder.
2. [loggervoices](https://github.com/SCANS-Survey/loggervoices) - a [PAMGuard plugin module](https://www.pamguard.org/pluginmodules.html) that captures voices from the app and records them to files whenever sightings buttons are pressed.

Configuration files, sample databases, etc. are in the [SCANS](https://github.com/SCANS-Survey/SCANS) repository. See the readme and wiki in that repository (under development) for instructions on how to set things up. 

Additional help material will (eventually) be incorporated into the PAMGuard help pages for [PAMGuard Logger Forms](https://www.pamguard.org/olhelp/visual_methods/loggerFormsHelp/docs/loggerFormsOverview.html), the Webcam capture module, etc. 
