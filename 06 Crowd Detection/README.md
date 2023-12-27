# **Crowd Detection**
 
***Steps to apply Crowd Detection Analytic***

1. Analytic Specific Settings
   - Select Object
2. Object Sizes
   - Draw People Size
   - Draw Crowd Area
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - No Zones will be drawn in Crowd Detection Analytics
   - Zone for Crowd Detection

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/06%20Crowd%20Detection/images/crowd%20detection.png "Camera Tampering")

4. Click on the crowd area zone and customize the max and min people count threshold
5. Check Alert When the Crowd People threshold reaches the limit
6. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/06%20Crowd%20Detection/images/crowd%20Alert.png "Camera TamperingOutput")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Crowd Detection
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\06 Crowd\crowd_canteen1
   - Draw People size, crowd area
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of the Crowd Detection when maximum crowd threshold reaches_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/06%20Crowd%20Detection/images/crowd%20detection.png "Camera Tampering")

2. No Crowd Detection
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\06 Crowd\no crowd_outside_farm1
   - Draw People size, crowd area
   - Check birth and death threshold in Advance Analytic Setting
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_NO alert will be generated because there is no crowd in this area_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/06%20Crowd%20Detection/images/no%20crowd%20detection.png "No Camera Tampering")

***Different test Cases only for Crowd Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
4. Enable the `Find Attributes` setting in Advance Analytic Settings
5. Detection with `isRule`
6. No Exchange of person ID
  
