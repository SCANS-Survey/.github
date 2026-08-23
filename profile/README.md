# SCANS Survey

These Github pages include software and instructions for running an advanced visual data collection system, primarily targetted at ship based visual line transect surveys for cetaceans.

The work builds on a system created by Doug Gillespie, Russell Leaper, et.al., for the 2005 SCANS II survey [An Integrated Data Collection System for Line Transect Surveys](https://doi.org/10.47536/jcrm.v11i3.601) 

This new iteration of the system brings in two important changes:

1. We now use [forms](https://www.pamguard.org/olhelp/visual_methods/loggerFormsHelp/docs/loggerFormsOverview.html) inside the [PAMGuard](www.pamguard.org) software instead of the out of date and unsupported [Logger 2000 ](https://www.marineconservationresearch.co.uk/downloads/logger-2000-rainbowclick-software-downloads/) software.
2. All of the wired buttons, webcams, microphones, etc. used by each observer have been replaced with a mobile phone app.

This means that (we hope) all components required to use this system can be bought off the shelf without any need to build and maintain bespoke hardware.  

This is a work in progress, targeting surveys in the summer of 2027, hopefully with testing at sea earlier that year, or possibly late 2026. 

This GitHub organisation will contain repositories of software developments specific to this survey method and also repositories of important configuration files and sample databases that you'll probably want to help get a system up and running. 

The main code development repositories are currently:

1. [scansapp](https://github.com/SCANS-Survey/scansapp) - an Android (phone or tablet) app that has sightings buttons, captures webcam images, location data (GPS), and sends voice to the PAMGuard data recorder.
2. [loggervoices](https://github.com/SCANS-Survey/loggervoices) - a [PAMGuard plugin module](https://www.pamguard.org/pluginmodules.html) that captures voices from the app and records them to files whenever sightings buttons are pressed.
3. [camergrabber](https://github.com/SCANS-Survey/cameragrabber) - a [PAMGuard plugin module](https://www.pamguard.org/pluginmodules.html) that can capture and store timestamped webcam images and images from the scansapp. We've previously used these to take images of lines on the deck, below the tracker binoculars, to measure angles.
4. [videocontrol](https://github.com/SCANS-Survey/videocontrol) - To control video cameras, used for video range tracking. 
5. [scansappnmea](https://github.com/SCANS-Survey/scansappnmea) - a [PAMGuard plugin module](https://www.pamguard.org/pluginmodules.html) that receives location data from the app in NMEA format. This means that the mobile device / scasnapp can be used in place of a normal GPS unit within PAMGuard.
6. [Validation](https://github.com/SCANS-Survey/validation) - Data validation code for use at sea and for offline processing.
7. Configuration files, sample databases, etc. are in the [SCANS](https://github.com/SCANS-Survey/SCANS) repository.

See the readme files in individual repositories and [wiki pages](https://github.com/SCANS-Survey/scansapp/wiki) (under development) for instructions on how to set things up. 

Additional help material will (eventually) be incorporated into the PAMGuard help pages for [PAMGuard Logger Forms](https://www.pamguard.org/olhelp/visual_methods/loggerFormsHelp/docs/loggerFormsOverview.html), the Webcam capture module, etc. 

All software developments are being released under the [GPL 3](https://choosealicense.com/licenses/gpl-3.0/) open source license, which basically means anyone can use and modify the software, but you should share back any improvements you make. Sample configurations are available under the [Creative Commons CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/legalcode.en) license, which means that you can really do what you want with these and have no obligation to share modifications. In short, this means that we want you to share improvements to the software, but we have no need to know what you're doing with it, or to have any access to, or knowledge of, the data you collect.

Citation. We'll eventually get a DOI of some sort to cite, but for now please either get in touch, or cite these GitHub pages. 

## Latest / Current Version - Quick download
| Package | Purpose | Latest |
|---------|---------|---------|
| [scansapp](https://github.com/SCANS-Survey/scansapp) | Android App | [scansapp_1.1.apk](https://github.com/SCANS-Survey/scansapp/releases/download/V1.1/scansapp_1.1.apk) |
| [loggervoices](https://github.com/SCANS-Survey/loggervoices) | Stream and capture observer audio from scansapp | [loggervoices1.0.jar](https://github.com/SCANS-Survey/loggervoices/releases/download/V1.0/loggervoices1.0.jar) |
| [camergrabber](https://github.com/SCANS-Survey/cameragrabber) | Grab camera frames from webcam or scansapp  for angle measurement | [cameragrabber-1.1.jar](https://github.com/SCANS-Survey/cameragrabber/releases/download/V1.1/cameragrabber-1.1.jar) |
| [videocontrol](https://github.com/SCANS-Survey/videocontrol)  | Control video cameras / recorders for range measurement | Not yet available |
| [scansappnmea](https://github.com/SCANS-Survey/scansappnmea)  | Capture NMEA (GPS) data from scansapp | [scansappnmea1.0.jar](https://github.com/SCANS-Survey/scansappnmea/releases/download/V1.0/scansappnmea1.0.jar) |
| [Validation](https://github.com/SCANS-Survey/validation) | Quality control during and after survey | Not yet available |

