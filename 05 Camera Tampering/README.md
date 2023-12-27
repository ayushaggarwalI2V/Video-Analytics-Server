# **Camera Tampering**
 
***Steps to apply Camera Tampering Analytic***

1. Analytic Specific Settings
   - Select Object
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - No Zones will be drawn in Camera Tampering Analytics

   - Zone for Camera Tampering

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/03%20Action%20Recognition/images/action%20Recg%20VMS.png "Camera Tampering")

4. Check Alert When the motion happens
5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. Check Frame Skipping and its effect on the computation of the system.
7. Check Moving senstivity ratio
8. Enable and Disable fog detetion
9. Pix Change Ratio
10. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/03%20Action%20Recognition/images/Fight%20detection.png "Camera TamperingOutput")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Outside Camera Tampering
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\05 Camera Tampering\cameraTampering Outside1
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of the Camera Tampered when camera is tampered_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/03%20Action%20Recognition/images/action%20outside.png "Camera Tampering")

2. No Camera Tampering
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\05 Camera Tampering\no camera tampering_city1
   - Check birth and death threshold in Advance Analytic Setting
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_NO alert will be generated because there is no camera tampered_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/03%20Action%20Recognition/images/road%20side%20action.png "Camera Tampering")

***Different test Cases only for Camera Tampering***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
4. Check Pixel Change ratio
5. Check Camera covered Alert
10. Advance Settings
  
