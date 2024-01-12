# **Action Recognition**
 
***Steps to apply Action Recognition Analytic***

1. Analytic Specific Settings
   - Select Object
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - No Zones will be drawn in Action Recognition Analytics

   - Zone for Action Recognition

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/03%20Action%20Recognition/images/action%20Recg%20VMS.png "VMS Action")

4. Check Alert When the fight or waving happens
5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. For Action Recognition [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/116)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/03%20Action%20Recognition/images/Fight%20detection.png "Action Recog Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Outside Action Video
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\03 Action Recog\outsideAction1
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of the Action when the fight is detected_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/03%20Action%20Recognition/images/action%20outside.png "Action")

2. Road Side Action
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\03 Action Recog\roadAction3
   - Check birth and death threshold in Advance Analytic Setting
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_Must get alert of the Action when the fight is detected_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/03%20Action%20Recognition/images/road%20side%20action.png "Action")

3. Gallery Action
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\03 Action Recog\galleryAction2
   - Also Check Waveing Alert 
   - Expected Output -> **Must get an alert of the Action when the fight is detected**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/03%20Action%20Recognition/images/action%20Recg%20VMS.png "Action")

***Different test Cases only for Action Recognition***

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
  
