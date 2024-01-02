![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/assets/153894100/bba5f36f-32ce-4c51-9cb0-8ab4dd0106f3)# **Smoke Detection**
 
***Steps to apply Smoke Detection Analytic***

1. Analytic Specific Settings
   - Select Object
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - No Specific Zones will be drawn in Smoke Detection Analytics

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/07%20Fire%20Detection/images/Fire%20VMs.png "Smoke Detection")

4. Check Alert When the Smoke shows in the video
5. For Smoke Detection [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/112)
6. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Smoke Interval -> event time between fire detects
9. Output will Look like

     ![image]( "Smoke Detection")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Smoke Detection (White Smoke)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\15 Smoke Detection\smoke_home_heavy1
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of the Smoke Detection_**
     
     ![image]( "Smoke Detection")

2. Smoke Detection (Black Smoke)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\15 Smoke Detection\smoke_fire_home_outside2
   - Check birth and death threshold in Advance Analytic Setting
   - Check the background similarity factor -> Check background to use background matching algorithm
   - Expected Output -> **_Must get alert of the Smoke Detection_**
   
     ![image]( "Smoke Detection")
     
3. No Smoke Detection
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\15 Smoke Detection\no smoke_fire_outside1
   - Expected Output -> **_NO alert will be generated because there is no Smoke in this area it has only fire_**
   
     ![image]( "No Smoke Detection")

***Different test Cases only for Smoke Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
