# 2018 Strategy System

This document will explain the various components in 1257's strategy system for 2018 (FIRST Power Up).

## Components of Strategy

### Objective Scouting
The goal of objective scouting is to collect quantitative data on all teams during competition.

#### Scouting App
For the 2018 season, Team 1257 created a scouting app for objective scouting. [outline system, describe google forms, data analysis, etc.]:

[scouting app screenshot]

##### Information Collected in Scouting App
1. **Event, Team #, Match #**: This information lets us know what is being scouted.
2. **Initials**: We collect the scout's initials so if there are any questions about the data, we know who to approach.
3. **Auto**
   1. **Cross Line**: Scouts should know the official definition of crossing the auto line.
   2. **Switch** and **Scale**: The choices are all numbers from 0-5. These questions count the number of cubes placed on the switch and scale in auto.
4. **Teleop**
   1. **Endgame**: The choices are Climbed, Tried to Climb, Parked, and None. Scouts should use their best judgment when determining if robots are trying to climb.
   2. **Climb Help**: Choices are Gave, Received, and None. Because the responses from the scouting app are vague, we usually rely on subjective scouts to provide a better description of endgames on Team 1257.
5. **Cube Things**: This section counts the number of cubes deposited in each of these locations: Switch, Scale, Opponent Switch, Exchange, and Dropped on Field.
6. **Notes**: In this section, scouts can write freeform notes to describe what happened in the match, provide context for the robot's actions, or describe the robot's performance. Suggested things to note include robot malfunctions, fouls, driving speed and ability, skill at defense, auto path, cube placement, intake reliability, climb type and reliability, and power-up usage.

##### Other Scouting App Components
1. **Objective / Pit Buttons**: These buttons don't currently do anything. If we create a pit scouting app in the future, these buttons can be used to switch between the two.
2. **Send Data**: This button will export the scouted matches in a modified .csv format. You can either display this exported data on the same device if there is internet, or you can send the data through Bluetooth to another device.
3. **Stored Matches Counter**: This number represents the number of unsent matches stored on the tablet. After sending data, this number should reset to 0.
4. **Reset Page**: Pressing this button twice will clear the page. However, it does not affect any matches that have already been submitted.
5. **Cancel**: If there is a red message below the top row of buttons and above the scouting assignment, pressing this button will remove that message.
6. **Scouting Assignment**: This shows which robot the scout is responsible for watching. The options are Red Nearest, Red Middle, Red Farthest, Blue Nearest, Blue Middle, and Blue Farthest, where Nearest, Middle, and Farthest refer to the robot's position on the field.
7. **Scouting Assignment Button**: This opens a dropdown menu that allows head scouts to change what is shown in the Scouting Assignment field. The buttons are blacked out to deter scouts from unintentionally changing this field.
8. **Submit Button**: This button should be pressed whenever a match has been fully scouted. After pressing this button, the app will display an error if any fields have been left blank. This is to make sure scouts don't forget to fill anything out. If everything has been filled out, it will store the data locally.

##### Using the Scouting App
To use the scouting app, you will need an Android tablet. To send data from the app, you will either need Internet access or a Bluetooth connection to a device with Internet access.

1. Open the latest version of the scouting app. You can find the .apk [here.](https://drive.google.com/open?id=1z5u0EEH1xg7zsRAD2hs8-02C9KJ4v9XR)
2. If the scouting app is being used at competition, specify which robot should be scouted by using the Scouting Assignment Button. This step is unnecessary for prescouting.
3. Make sure scouts know how to use the app. Also, make sure scouts know what to include in Notes, because good notes are very important in fully understanding a robot's capabilities. On Team 1257, we hold a scouting training session towards the end of build season, and we also have head scouts teach people at competition if necessary.
4. After an appropriate number of matches, send data from the app. Instructions for sending data are given below.

##### How to Send Data
If your tablet has Internet:

1. Click the "Send Data" button.
2. Select "This Device".
3. The data should appear in the Notes box. Select all of the data and choose Cut.
4. Open the Google Form for your data analysis spreadsheet. For reference, ours is located [here.](https://docs.google.com/forms/d/e/1FAIpQLSc3q8jLCsXbG86QdCjSnhLQb-dfINtFVXdnw7TE3kJe5hQHhw/viewform)
5. Paste the data and submit the form. The data should now be in Google Sheets for processing.

If you have another Android tablet with Internet:

1. Make sure the two devices are paired with Bluetooth.
2. Open the scouting server on the Android tablet with Internet. You can find the .apk [here.](https://drive.google.com/open?id=1z5u0EEH1xg7zsRAD2hs8-02C9KJ4v9XR)
3. Click "Accept Connections" on the scouting server.
4. On the scouting app, click the "Send Data" button.
5. Select the device with the scouting server.
6. The data should appear in a large text box on the scouting server. Select all of the data and choose Cut.
7. Open the Google Form for your data analysis spreadsheet. For reference, ours is located [here.](https://docs.google.com/forms/d/e/1FAIpQLSc3q8jLCsXbG86QdCjSnhLQb-dfINtFVXdnw7TE3kJe5hQHhw/viewform)
8. Paste the data and submit the form. The data should now be in Google Sheets for processing.

## Members Involved
* **6 Objective Scouts**: Objective scouts will use the scouting app during matches. One objective scout is responsible for each robot. If there are enough people, it's usually a good idea to rotate scouts in and out so people can get breaks. On Team 1257, we create a rotating schedule for each competition to evenly distribute roles throughout the team.
* **Pit Scouts**: Pit scouts will ask teams about their robots at the start of competition. For each team they approach, the pit scouts will complete a pit scouting sheet with information about their robot. On Team 1257, pit scouts are typically responsible for 8-12 teams, and they go in pairs (usually 1 experienced pit scout and 1 new pit scout).
* **Subjective Scouts**: Subjective scouts take freeform notes on robots during matches. Usually, subjective scouts will note more qualitative data points, while objective scouts will note more quantitative data points. On Team 1257, the most trusted objective scouts from the previous year are usually chosen to be subjective scouts.
* **Leadership**: On Team 1257, the leadership is responsible for organizing scouts, enforcing the schedule, answering questions about the strategy system, and sending data from the tablets. On Team 1257, there is one strategy captain and two head scouts, but in addition to this, subjective scouts can be in leadership roles as well because they are the most trusted members of strategy.
