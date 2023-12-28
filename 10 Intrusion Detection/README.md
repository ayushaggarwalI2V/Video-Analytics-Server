# **Intrusion Detection**
 
***Steps to apply Intrusion Detection Analytic***

1. Analytic Specific Settings
   - Select Filtered Object
   - Select Object
2. Object Size
   - Draw Min and Max Size of the Object
4. Drawing Setting
   - Draw ROI
   - Draw Zone for Intrusion Detection

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/10%20Intrusion%20Detection/images/intrusion%20outside.png "Intrusion Detection")

5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. Check Frame Skipping and its effect on the computation of the system.
7. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/10%20Intrusion%20Detection/images/alert%20intrusion.png "Intrusion Detection output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Intrusion Outside
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\09 Garbage detection\garbage_night_day2
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Alert must be generated when garbage detects_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/10%20Intrusion%20Detection/images/intrusion%20outside.png "Intrusion Detection")

2. Intrusion Detection Crawl
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\09 Garbage detection\garbage_outside1
   - Check the confidence value
   - Expected Output -> **_Alert must be generated when garbage detects_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/10%20Intrusion%20Detection/images/intrusion%20crawl.png "Garbage Detection")

3. Intrusion Detection IOCL
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\09 Garbage detection\garbage_outside1
   - Check the confidence value
   - Expected Output -> **_Alert must be generated when garbage detects_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/10%20Intrusion%20Detection/images/intrusion%20iocl.png "Garbage Detection")

***Different test Cases only for Intrusion Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping in `Analytic Advance Setting`
4. Check the confidence value in `Analytic Specific Setting`
5. Enable `Find Attributes` in Analytic Advance setting
