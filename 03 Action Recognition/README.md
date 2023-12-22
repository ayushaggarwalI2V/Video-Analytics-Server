# **Action Recognition**
 
***Steps to apply Action Recognition Analytic***

1. Analytic Specific Settings
   - Select Object
   - For No Motion
     - No Motion Interval - Time in seconds for no motion
     - No Motion Alert Interval - Interval in sec for No motion alerts
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - No Zones will be drawn in Motion Analytics

   - Zone for Motion Detection

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/02%20Advance%20Motion/images/advanceMotionVMS.png "VMS Motion")
     
   - Zone for No Motion
    
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/02%20Advance%20Motion/images/noMotion%20VMS.png "VMS no Motion")
     
4. Check Alert When the motion happens
5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like
   - For Motion Alert

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/02%20Advance%20Motion/images/MotionAlert.png "No Motion Output")
     
   - For No Motion Alert
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/02%20Advance%20Motion/images/noMotionAlert.png "No Motion Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Canteen Motion Video
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\02 Advance Motion\canteenMotion1
   - Disable `checkNoMotion` in Analytic Specific Setting
   - Enable `CheckMotion` in Analytic Specific Setting
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of the motion object_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/02%20Advance%20Motion/images/advanceMotionVMS.png "Canteen Motion")

2. City Scenario (City Motion Detection)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\02 Advance Motion\cityMotion2
   - Disable `checkNoMotion` in Analytic Specific Setting
   - Enable `CheckMotion` in Analytic Specific Setting
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_Alert of the All Motion Object is generated_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/02%20Advance%20Motion/images/city%20motion%20detection.png "City Motion")

3. No Motion Detection
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\01 Abandon\highwayAbandon 1
   - Enable `checkNoMotion` in Analytic Specific Setting
     - No Motion Setting in the Analytic Specific Setting
       - No Motion Interval - 10 Sec
       - Time in seconds for no motion - 2 Sec
     - No Motion Alert Interval - Interval in sec for No motion alerts 
   - Disable `CheckMotion` in Analytic Specific Setting
   - Check Alert for the No Motion by No Motion Interval
   - Must check Motion Detection Alert not coming because we disabled the `checkMotion` setting
   - Expected Output -> **Must get alert of No Motion**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/02%20Advance%20Motion/images/noMotion%20VMS.png "No motion")

***Different test Cases only for Advance Motion***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
4. Check Bbox
5. Tracking of object -> ID persists, no exchange of ID
6. VA Stream Delay
7. Selected Object Settings in Analytic Specific setting -> car, bicycle, person, etc
8. Check Find Attributes in Analytic Advance Specific Setting
9. Show tracks, trackID
10. Advance Settings

***Must Check Setting***
- Enable `find Attributes` Setting in Analytic Advance Specific Setting by enabling `show advance prop.`
   - In the event card check attributes like -> backpack, bottom RGB (Bottom color), hat, longhair, longpants, longsleeves, etc
  
