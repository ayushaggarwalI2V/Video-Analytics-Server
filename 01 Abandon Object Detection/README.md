# **Abandon Object Detection**

***Steps to apply Abandon Analytic***

1. Analytic Specific Settings
   - Select Object
   - Check Stationary Duration Time 
   - Check Filter by Classification - To get alerts of only Selected items
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Zones (Shown in image)
   
    ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/vms%20abandon%20image.png "VMS image")

4. Check Alert When Object arrives and Stationary Duration
5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. For Abandon Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/114)
7. Check Frame Skipping and its effect on the computation of the system.


***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Graffiti Abandon Object
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\abandonGraffiti1
   - Remove filter event by classification
   - Check the stationary duration time
   - Draw the area as shown in the image
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/graffiti.png "Graffiti Abandon")

2. City Scenario (City Abandon)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\cityAbandon 3
   - Remove filter event by classification
   - Check the stationary duration time
   - Check Alert for bag after the Stationary duration time
   - Check the background similarity factor
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/cityAbandon.png "City Abandon")

3. Highway Scenario
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\highwayAbandon 1
   - Set stationary duration time to 10 sec
   - Check Alert for on=bject after the Stationary duration time
   - Must check other objects not showing the abandoned object
   - Check with different select objects like - cars, buses, etc
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/highwayAbandon%201.png "Highway Abandon")

4. No Abandon - no alert generated 
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\no abandon 1
   - Set stationary duration time to 10 sec
   - *Must check no alert is generated because there is no abandoned item in this video*
   - Must check other objects not showing the abandoned object
   - Check with different select objects like - cars, buses, etc
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/noabandoned.png "No Abandon")

***Different test Cases***
1. Check Release Update
2. Release clean install
3. Detection of different models
4. Check Backend -> Inference, Open CV, CUDA
5. Frame Skipping
6. Check Bbox
7. Tracking of object -> ID persists, no exchange of ID
8. VA Stream Delay
9. Advance Settings
