# **Face Detection**
 
***Steps to apply Face Detection Analytic***

1. Analytic Specific Settings
   - Select `Face` from Select Object
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - No Zone will be drawn for Face Detection

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/06%20Crowd%20Detection/images/crowd%20detection.png "Face Detection")

4. Click Detection on Different Confidence value
5. Check Alert When the Crowd People threshold reaches the limit
6. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/06%20Crowd%20Detection/images/crowd%20Alert.png "Face Detection")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Face Detection Real Time
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\08 Face\faceRealTime1
   - Draw People size, crowd area
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of the Face Detection_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/06%20Crowd%20Detection/images/crowd%20detection.png "Face Detection")

2. Face Detection (Sequence Wise Images Combination)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\08 Face\face_pictures1
   - Draw People size, crowd area
   - Check birth and death threshold in Advance Analytic Setting
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_Must get alert of the Face Detection_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/06%20Crowd%20Detection/images/no%20crowd%20detection.png "Face Detection")

***Different test Cases only for Face Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
4. Enable the `Find Attributes` setting in Advance Analytic Settings
5. Detection with `isRule`
6. No Exchange of person ID
  
