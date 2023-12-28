# **Garbage Detection**
 
***Steps to apply Garbage Detection Analytic***

1. Analytic Specific Settings
   - Select Object
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Zone for Garbage Detection

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/09%20Garbage%20Detection/images/garbage%20detection.png "Garbage Detection")

4. For detailed information of Garbage Detection [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/118)
5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. Check Frame Skipping and its effect on the computation of the system.
7. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/09%20Garbage%20Detection/images/alert%20garbage%20detection.png "Garbage Detection output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Garbage Detection (Day & Night)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\09 Garbage detection\garbage_night_day2
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Alert must be generated when garbage detects_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/09%20Garbage%20Detection/images/garbage%20detection.png "Garbage Detection")

2. Garbage Detection Outside Scenario
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\09 Garbage detection\garbage_outside1
   - Check the confidence value
   - Expected Output -> **_Alert must be generated when garbage detects_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/09%20Garbage%20Detection/images/garbage%20outside.png "Garbage Detection")

***Different test Cases only for Garbage Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping in `Analytic Advance Setting`
4. Check the confidence value in `Analytic Specific Setting`
