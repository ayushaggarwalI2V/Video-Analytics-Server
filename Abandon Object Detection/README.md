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
   
    ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/Abandon%20Object%20Detection/images/vms%20abandon%20image.png "VMS image")

4. Check Alert When Object arrives and Stationary Duration
5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. For Abandon Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/114)


***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Graffiti Abandon Object
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\abandonGraffiti1
   - Remove filter event by classification
   - Check the stationary duration time
   - Draw the area as shown in the image
   - Check this for more information [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/114)
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/Abandon%20Object%20Detection/images/graffiti.png "Graffiti Abandon")

2. City Scenario (City Abandon)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\cityAbandon 3
   - Remove filter event by classification
   - Check the stationary duration time
   - Check Alert for bag after the Stationary duration time
   - Check this for more information [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/114)
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/Abandon%20Object%20Detection/images/cityAbandon.png "City Abandon")
