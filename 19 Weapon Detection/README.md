# **Weapon Detection**
 
***Steps to apply Weapon Detection Analytic***

1. Analytic Specific Settings
   - Select Object
   - Select Model
2. Object Size
   - Draw Min and Max Size of the Object
4. Drawing Setting
   - Draw ROI
   - No Specific Zone will be drawn

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/19%20Weapon%20Detection/images/weapon%20realtime.png "Weapon Detection")

5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. Check Frame Skipping and its effect on the computation of the system.
7. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/19%20Weapon%20Detection/images/weapon%20alert.png "Weapon Detection output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Weapon Detection Realtime Scenario
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\19 Weapon\weapon_shotgun1
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Alert must be generated when weapon detects_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/19%20Weapon%20Detection/images/weapon%20realtime.png "Weapon Detection")

2. Weapon Detection Robotic
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\19 Weapon\weapon_robot_gun2
   - Expected Output -> **_Alert must be generated when weapon detects_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/19%20Weapon%20Detection/images/weapon%20robotic.png "Weapon Detection")

3. No Weapon Detection
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\19 Weapon\no weapon_City1
   - Check the confidence value
   - Expected Output -> **_No Alert must be generated when the weapon detects_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/19%20Weapon%20Detection/images/no%20weapon.png "Weapon Detection")

***Different test Cases only for Weapon Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping in `Analytic Advance Setting`
4. Check the confidence value in the `Analytic Specific Setting`
