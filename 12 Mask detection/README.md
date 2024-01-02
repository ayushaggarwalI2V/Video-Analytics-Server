# **Mask Detection**
 
***Steps to apply Mask Detection Analytic***

1. Analytic Specific Settings
   - FPS
   - Select Object -> head, face
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Zone

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/12%20Mask%20detection/images/mask%20detection.png "Mask Detection")

4. Mask Classification Model -> Used to detect masks on face 
5. Check Alert
6. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/12%20Mask%20detection/images/no%20mask%20canteen.png "Mask Detection Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Mask Detection (Canteen Video)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\12 Mask\mask_canteen1
   - Draw zone
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of no mask face_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/12%20Mask%20detection/images/mask%20detection.png "Mask Detection")

2. Mask Detection (Outside Video)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\12 Mask\no mask_outside1
   - Set `frame skipping` to 3 by enabling `show advance setting` 
   - Expected Output -> **_Must get alert of no mask face_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/12%20Mask%20detection/images/mask%20detection%20outside.png "No Mask Detection")

***Different test Cases only for Mask Detection***

1. Detection with face different models - face1, face2 ...
2. Detection with different Mask Classification Model
3. Frame Skipping
4. Check with different value of confidence
5. Different values `Birth and Lost thresold` in Advance Analytic Setting 
