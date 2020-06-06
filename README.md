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

It roughly costs over 8000 to 10000.

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
The system can also provide it with three features like
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

*product requirements:*
the system restarts once for every 6 hours of working, which will flush all the cache.
additional to this we need to run the monthly updates.
as the lifespan of the pi camera is less compared to raspberry pi we need to change it once every 5 years.

organiational requirements
one can create an account/login using his driving license.

The version control system  which we are using is git.
To make the python scripts standalone we are using a package called pyinstaller.
Unit testing tools which we arre going to use are: pytest, doctest
Continuous integration will be done by Travis CI.

**Constraints**
There should be enough light to detect the pothole, and car should be moving with a average speed of 40-60km/hr to get a good quality of the video.

Dataset link: [link](https://www.kaggle.com/sachinpatel21/pothole-image-dataset)

*Validation testing:* For validation tests we use the images which we have collected from sites to check wheather all the scripts are bug free.
This will also be carried out during the demonstartion to our stakeholders(excluding developers).

*Defect testing:* For defect testing we record some real world videos of road and present it, which not only includes images of road but, also images of some patterns which are similar to potholes, to measure how accurate is it detecting potholes, when both potholes and potholes like patterns are present.

**Risk Mitigation**
one of the risk which the device faces is external accidents/shocks which are unpredictables
example:
* Someone hitting it
* Snow covering the lens
* camera being covered by some object.
* Rain water going into the circuits and frying them.

## Possible Extensions

1) To make it budget friendly.
2) Reduce the latency between the uploads.
3) Detect potholes even when the car is at very high speed.