# Pothole Detection

Software Project Management Plan
This document serves as the project plan for the Pothole detection. The content of this document is divided into ___ chapters: .

## Introduction

**Statement:**
Pothole detection and alter system which detects potholes on the road raspberry pi and pi camera and updates in google maps.

**Team**

* Anurag Peddi(17MCME13)

* Yagnahaun Jonnadula(17MCME23)

**Imapct**

Over the last five years, the number of deaths caused by the potholes are around 15000, if we can implement this system and use it, then there is a chance that we can reduce the number of deaths.

**Budget**

It roughly costs over 6000 to 7000.

## Further Analysis

**Stakeholders**

* User

* DataAnalyst who takes the data provided by the devices and perform some data analysis stuff.

* Software Developer who debugs any issues after the installation

* Company which produces these systems

* IT Staff who installs and maintain the system.

### Requirenments

**System Functions**
The embedded device processes the incoming stream of video and detects any pothole in the stream, if any it immediately intimates the user with a signal.

It also saves, the information of pothole detection and coordinates in a file for cross validation.

*Functional Requirements:*
The system can also provide it with two features like
* Detect pothole and Alert driver

* Just Detect the pothole

* Just alert the driver

type of software which we are going to use is python scripts, drivers are our expected users, are going to use this in embedded systems.

functional user requirements
    pass

fuunctional system requirements
    pass

*Non-Functional Requirements:*
As we are using a pretrained model for detecting the potholes, the time contraint will only be on alerting the driver.

product requirements
the system restart once for every 6 hours of working, which will flush all the cache.
additional to this we need to run the monthly updates.
as the lifespan of the pi camera is less compared to raspberry pi we need to change it once every 5 years.

organiational requirements
one can create an account/login using his driving license.

**Constraints**
There should be enough light to detect the pothole, and car should be moving with a average speed of 40-60km/hr to get a good quality of the video.