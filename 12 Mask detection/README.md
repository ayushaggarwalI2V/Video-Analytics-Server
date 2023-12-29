# **Mask Detection**
 
***Steps to apply Mask Detection Analytic***

1. Analytic Specific Settings
   - FPS
   - Match Threshold -> threshold value specifies the maximum acceptable number of comparisons
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Rects on the object (for multiple objects draw multiple rects on the objects)

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/11%20Missing%20Object%20Detection/images/missing%20object%20.png "Mask Detection")

5. Check Alert When the object missed in the video
6. Learning-based algorithm first it will learn the frames and then detect the missing objects
7. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
8. Check Frame Skipping and its effect on the computation of the system.
9. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/11%20Missing%20Object%20Detection/images/alert%20missing%20object.png "Mask Detection Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Missing Object Detection (3 Different Objects Scenario)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\11 MissingObject\missingObject_office1
   - Draw 3 rects for 3 objects
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get 3 alerts of the Mask Detection_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/11%20Missing%20Object%20Detection/images/missing%20object%20.png "Mask Detection")

2. No Missing Object Detection
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\11 MissingObject\no missingObject_office1
   - Draw People size, crowd area
   - Check birth and death threshold in Advance Analytic Setting
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_NO alert will be generated because there is no missing object in this area_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/11%20Missing%20Object%20Detection/images/missing%20object%20.png "Mask Detection")

***Different test Cases only for Mask Detection***

1. Detection with different models
2. Frame Skipping
3. Check with different match threshold in the `Analytic Specific Setting`
4. Missing Duration time `Analytic Specific Setting`
