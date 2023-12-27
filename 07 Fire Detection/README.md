# **Fire Detection**
 
***Steps to apply Fire Detection Analytic***

1. Analytic Specific Settings
   - Select Object
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - No Zones will be drawn in Fire Detection Analytics

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/07%20Fire%20Detection/images/Fire%20VMs.png "Fire Detection")

4. Check Alert When the Fire shows in the video
5. For Fire Detection [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/110)
6. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Fire Interval -> event time between fire detects
9. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/07%20Fire%20Detection/images/fire%20alert.png "Fire Detection")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Fire Detection
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\07 Fire\fire_building1
   - Enable `color first`
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of the Fire Detection_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/07%20Fire%20Detection/images/Fire%20VMs.png "Fire Detection")

2. Fire Detection (Crash Scene) 
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\07 Fire\fire_crash2
   - Check birth and death threshold in Advance Analytic Setting
   - Check the background similarity factor -> Check background to use background matching algorithm
   - Expected Output -> **_Must get alert of the Fire Detection_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/07%20Fire%20Detection/images/Fire%20crash.png "Fire Detection")

3. Fire Detection House
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\07 Fire\fireAndSmoke_home_outside3
   - Check birth and death threshold in Advance Analytic Setting
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_Must get alert of the Fire Detection_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/07%20Fire%20Detection/images/fire%20house.png "Fire Detection")
     
4. No Fire Detection
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\07 Fire\no fire_smoke_home1
   - Disable `Check CA`
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_NO alert will be generated because there is no fire in this area it has only smoke_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/07%20Fire%20Detection/images/no%20fire.png "No Fire Detection")

***Different test Cases only for Fire Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
4. Detection with `colorFirst`
5. Detection with `checkCA`
