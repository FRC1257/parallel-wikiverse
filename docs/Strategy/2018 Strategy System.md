# 2018 Strategy System

This document will explain the various components in 1257's strategy system for 2018.

## Components of Strategy

### Objective Scouting
The goal of objective scouting is to collect quantitative data on all teams during competition.

#### Scouting App
For the 2018 season, Team 1257 created a scouting app. [describe google forms, data analysis, etc.]:

[scouting app screenshot]

Team 1257 collects the following information in our scouting app:
1. Event, Team #, Match #: This information lets us know what is being scouted.
2. Initials: We collect the initials of the scout so if there are any questions about the data, we know who to approach.
3. Auto
a. Cross Line: Make sure scouts know the official definition of crossing the auto line.
b. Switch and Scale: Choices are all numbers from 0-5.
Number of cubes placed on these components in auto.
4. Teleop
a. Endgame: Choices are Climbed, Tried to Climb, Parked, and None.
This question can be ambiguous, so scouts will have to use their best judgment.
b. Climb Help: Choices are Gave, Received, and None.
This question is also ambiguous. Subjective scouts should be able to provide a better description of a robot's endgame.
5. Cube Things
This section counts the number of cubes a robot uses in each of these objectives: Switch, Scale, Opponent Switch, Exchange, and Dropped on Field.
6. Notes
In this section, scouts can write freeform notes to elaborate on things that happened in the match, provide context, or describe the robot's performance. Suggested things to note include robot malfunctions, fouls, driving speed and ability, auto path, cube placement, intake reliability, climb type and reliability, and power-up usage.

Other components of the scouting app include:
1. Objective / Pit Buttons: These buttons don't currently do anything. If we create a pit scouting app in the future, these buttons will switch between the two.
2. Send Data: This button will export the scouting data in a modified .csv format. You can either display this exported data on the same device if there is internet, or you can send the data through Bluetooth to another device.
3. Stored Matches Counter: This number represents the number of submitted matches stored on the tablet. After sending data, this number should reset to 0.
4. Reset Page: Pressing this button twice will clear the page. However, it does not affect any matches that have already been submitted.
5. Cancel: If there is a red message below the top row of buttons and above the scouting assignment, pressing this button will remove that message.
6. Scouting Assignment: This shows which robot that scout is responsible for watching. Red or Blue refers to the alliance, and Nearest, Middle, and Farthest refers to robot position on the field. For example, Blue Middle refers to the middle blue robot on the field.
7. Scouting Assignment Button: This opens a dropdown that allows you to change what is shown in the Scouting Assignment. The buttons are blacked out to prevent scouts from unintentionally changing this field.
8. Submit Button: Press this button after a match is done being scouted. This button can only be pressed if all fields in the scouting app are filled in. This is to make sure scouts don't forget to fill anything out. After pressing the submit button, the Stored Matches Counter should increase by 1.

To use the scouting app, you will need an Android tablet and a poor soul who is willing to scout. To send data from the app, you will either need Internet access or a Bluetooth connection to a device with Internet access.

Using the scouting app:
1. Open the latest version of the scouting app. You can find the .apk here: https://drive.google.com/open?id=1z5u0EEH1xg7zsRAD2hs8-02C9KJ4v9XR
2. If the scouting app is being used at competition, specify which robot should be scouted by using the Scouting Assignment Button. This step is unnecessary for prescouting.
3. Make sure scouts know how to use the app. Also, make sure scouts know what to include in Notes, because good notes are very important in fully understanding a robot's capabilities. On Team 1257, we hold a scouting training session towards the end of build season, and we also have head scouts teach people at competition if necessary.
4. After an appropriate number of matches, send data from the app. Instructions for sending data are given below.

To send data:
1. If your tablet has Internet:
a. Click the "Send Data" button.
b. Select "This Device".
c. The data should appear in the Notes box. Select all of the data and choose Cut.
d. Open the Google Form for your data analysis spreadsheet. For reference, ours is located here: https://docs.google.com/forms/d/e/1FAIpQLSc3q8jLCsXbG86QdCjSnhLQb-dfINtFVXdnw7TE3kJe5hQHhw/viewform
e. Paste the data and submit the form. The data should now be in Google Sheets for processing.

2. If you have another Android tablet with Internet:
a. Make sure the two devices are paired with Bluetooth.
b. Open the scouting server on the Android tablet with Internet. You can find the .apk here: https://drive.google.com/open?id=1z5u0EEH1xg7zsRAD2hs8-02C9KJ4v9XR
c. Click "Accept Connections" on the scouting server.
d. On the scouting app, click the "Send Data" button.
e. Select the device with the scouting server.
f. The data should appear in a large text box on the scouting server. Select all of the data and choose CUt.
g. Open the Google Form for your data analysis spreadsheet. For reference, ours is located here: https://docs.google.com/forms/d/e/1FAIpQLSc3q8jLCsXbG86QdCjSnhLQb-dfINtFVXdnw7TE3kJe5hQHhw/viewform
h. Paste the data and submit the form. The data should now be in Google Sheets for processing.

## Members Involved
* 6 objective scouts
Objective scouts will use the scouting app during matches. One objective scout is responsible for each robot. If there are enough people, it's usually a good idea to rotate scouts in and out so people can get breaks. On Team 1257, we create a rotating schedule for each competition to evenly distribute roles throughout the team.
* Pit scouts
Pit scouts will ask teams about their robots at the start of competition. For each team they approach, the pit scouts will complete a pit scouting sheet with information about their robot. On Team 1257, pit scouts are typically responsible for 8-12 teams, and they go in pairs (usually 1 experienced pit scout and 1 new pit scout).
* Subjective scouts
Subjective scouts will take freeform notes on robots during matches. Usually, subjective scouts will note more qualitative data points, while objective scouts will note more quantitative data points. On Team 1257, the most trusted objective scouts from the previous year are usually chosen to be subjective scouts.
* Leadership
On Team 1257, the leadership is responsible for organizing scouts, enforcing the schedule, answering questions about the strategy system, and sending data from the tablets. On Team 1257, there is one strategy captain and two head scouts, but in addition to this, subjective scouts can be in leadership roles as well because they are the most trusted members of strategy.
