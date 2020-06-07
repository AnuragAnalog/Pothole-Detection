# Pothole detection

Software Project Management Plan
This document serves as the project plan for the Pothole detection. The content of this document are divided into 7 chapters:

## Chapter-1(Introduction)

### Statement

Pothole detection and alert system which detects potholes on the road raspberry pi and pi camera and updates in google maps.

### Team

* Anurag Peddi(17MCME13)

* Yagnahaun Jonnadula(17MCME23)

### Imapct

In this fast moving world, people want to reach their destinations as soon as possible. There are some apps that suggests us the routes which can make us reach our destination early and there are some apps that shows the all possible routes with traffic congustion for whatever reason it may be, such as google maps and many more. 
But there are less number of apps that tells the condition of the road whether it is good to travel or not, whether it suggests the route to the driver based on the condition of the road. So this model mainly focuses on the travel safety of the passengers and update the passengers with the best route to travel.

Over the last five years, the number of deaths caused by the potholes are around 15000, if we can implement this system and use it, then there is a chance that we can reduce the number of deaths.

### Budget
It roughly costs over 8000 to 10000, which includes raspberry pi, pi camera, and it's accessories.

| Equipment | Estimated Cost |
| --- | --- |
| Raspberry Pi | 5000 |
| Pi Camera | 1000 |
| Accessories | 3000 |

## Chapter-2(Analysiss)

### Stakeholders

* User(driver)

* DataAnalyst who takes the data provided by the devices and perform some data analysis stuff.

* Software Developer who debugs any issues after the installation

* Company which produces these systems

* IT Staff who installs and maintain the system.

### Requirements
The embedded device processes the incoming stream of video and detects any pothole in the stream, if any it immediately intimates the user with a signal.

It also saves, the information of pothole detected and coordinates in a file for cross validation.

*Functional Requirements:*

The system can also provide it with three features like:
* Detect pothole and Alert driver

* Just Detect the pothole

* Just alert the driver

Type of software which we are going to use is python scripts, drivers are our expected users, are going to use this in embedded systems.

*functional user requirements*
    pass

*functional system requirements*
    pass

*Non-Functional Requirements:*

As we are using a pretrained model for detecting the potholes, the time contraint will only be on alerting the driver.

*product requirements:*

The system restarts once for every 6 hours of working, which will flush all the cache, additional to this we need to run the monthly updates to keep the software upto date.
As the lifespan of the pi camera is less compared to raspberry pi we need to change it once every 5 years.

*Organiational requirements*
One can create an account/login using his driving license.

## Chapter-3

## Chapter-4

### Testing
*The automation of the model goes on this process:*
The sensor nodes on the car and the GPS reciever can detect or identify the potholes on the early note or the manual recordings are used to update the location of the pothole to the data file which runs through a pothole detection algorithm which then can give the accurate postion of the detected potholes.

*Unit testing:* Unit testing tools which we are going to use are: pytest, doctest

*Validation testing:* For validation tests we use the images which we have collected from sites to check wheather all the scripts are bug free.
This will also be carried out during the demonstartion to our stakeholders(excluding developers).

*Defect testing:* For defect testing we record some real world videos of road and present it, which not only includes images of road but, also images of some patterns which are similar to potholes, to measure how accurate is it detecting potholes, when both potholes and potholes like patterns are present.

## Chapter-5

The version control system  which we are using is git.
To make the python scripts standalone we are using a package called pyinstaller.

## Chapter-6

### Schedule
*Time Line for development of this model:*

| Milestone | Date | Description |
| --- | --- | --- |
| Milestone 1 | March 12 | First phase Idea completion. |
| Milestone 2 | April 19 | Completeion of the planning of designing the model (Desing of the working the model) |
| Milestone 3 | Date | Gathering all the units required for the model. |
| Milestone 4 | Date | Assembling the units to a well designed model. |
| Milestone 5 | Date | Testing the model with all the data sets. |
| Milestone 6 | Date | Final model that is ready to deliver. |

### Risk
*Hardware*
One of the risk which the device faces is external accidents/shocks which are unpredictables
Example:
* Someone hitting it
* Snow covering the lens
* camera being covered by some object(paper).
* Rain water going into the circuits and frying them.

*Software*
The other kind of risks which the device faces is privacy and security of data.
The data should be transmitted only in a secure environment.

### Risk Mitigation
*Hardware*
If the device is enclosed in a box like structure then, some of the above risks can be avoided.

*Software*

## Chapter-7
### Possible extensions
1. To make it budget friendly.
2. Reduce the latency between the uploads.
3. Detect potholes even when the car is at very high speed.

**Constraints**
There should be enough light to detect the pothole, and car should be moving with a average speed of 40-60km/hr to get a good quality of the video.

Dataset link: [link](https://www.kaggle.com/sachinpatel21/pothole-image-dataset)