# **Advance Motion Detection**
 
***Steps to apply Motion Analytic***

1. Analytic Specific Settings
   - Select Object
   - Check Stationary Duration Time                                 
   - Check Filter by Classification - To get alerts of only Selected items
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Zones (Shown in image)
   
    ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/graffiti.png "VMS image")
   
4. Check Alert When Object arrives and Stationary Duration
5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. For Abandon Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/114)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/abandoned_graffiti_output.png "Abandon Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Graffiti Abandon Object
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\abandonGraffiti1
   - Disable `filter event by classification`
   - Check the stationary duration time
   - Draw the area as shown in the image
   - Expected Output -> **_Must get alert of object_** after the stationary duration time
     
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/graffiti.png "Graffiti Abandon")

2. City Scenario (City Abandon)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\cityAbandon 3
   - Disable `filter event by classification`
   - Check the stationary duration time
   - Check Alert for bag after the Stationary duration time
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_Alert of the bag is generated_**
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/cityAbandoned.png "City Abandon")

3. Highway Scenario
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\highwayAbandon 1
   - Set stationary duration time to 10 sec
   - Check Alert for the object after the Stationary duration time
   - Must check other objects not showing the abandoned object
   - Check with different select objects like - cars, buses, etc
   - Expected Output -> **_Must get alert of object_**
     
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/highwayAbandoned.png "Highway Abandon")

4. No Abandon - no alert generated 
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\no abandon 1
   - Set stationary duration time to 10 sec
   - *Must check no alert is generated because there is no abandoned item in this video*
   - Must check other objects not showing the abandoned object
   - Check with different select objects like - cars, buses, etc
   - Expected Output -> **_No alerts are generated_** because there is no abandoned object in this video
     
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/no%20abandoned.png "No Abandon")

***Different test Cases only for Abandon***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
4. Check Bbox
5. Tracking of object -> ID persists, no exchange of ID
6. VA Stream Delay
7. Filter by classification objects
8. Draw Multiple zones, min-max setting
9. Check Find Attributes
10. Show tracks, trackID
11. Advance Settings
