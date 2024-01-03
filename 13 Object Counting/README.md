# **Object Counting**
 
***Steps to apply Object Counting Analytic***

1. Analytic Specific Settings
   - FPS
   - Select Object -> car, bus, person, truck, etc.
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Counting Line -> Make direction by right click on the arrow (allow from both directions, toggle direction)
   - We can draw multiple counting lines as per the requirement
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/13%20Object%20Counting/images/object%20counting.png "Object Counting")

5. Check Alert
6. For Object Counting Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/120)
7. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
8. Check Frame Skipping and its effect on the computation of the system.
9. Check gender in the Analytic Specific setting -> Check this checkbox to get the gender description in person detection.
10. Output will Look like -> also shows total entered and exited object

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/13%20Object%20Counting/images/object%20counting%20alert.png "Object Counting Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Object Counting (Person Video)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\13 Object Counting\objectCounting_person_canteen1
   - Draw Perimeter Line
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of Object Entered or Exited when object Cross the counting line_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/13%20Object%20Counting/images/object%20counting.png "Object Counting")

2. Object Counting (Vehicles Video)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\13 Object Counting\objectCountingVehicle_city2
   - Select objects such as - car, bike, truck, auto
   - `Disable check gender` setting from analytic specific setting
   - Draw Perimeter line
   - Set `frame skipping` to 3 by enabling `show advance setting` 
   - Expected Output -> **_Must get alert of Object Entered or Exited when object Cross the counting line_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/13%20Object%20Counting/images/object%20counting%20vehicles.png "Object Counting")

***Different test Cases only for Object Counting***

1. Detection with different models - model1, model2...
2. Check the `backend` in analytic specific setting with OpenCV, CUDA, Inference Engine
3. Frame Skipping
4. Check with different values of confidence
5. Different values `Birth and Lost threshold` in Advance Analytic Setting 
