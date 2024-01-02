# **Social Distancing Detection**
 
***Steps to apply Social Distancing Detection Analytic***

1. Analytic Specific Settings
   - Select Object
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Zones for Social Distancing Detection
   - Draw Social distance line -> The distance between individuals

     ![image]( "Social Distancing Detection")

4. Check Alert When the social distance below the input value
5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. Check Frame Skipping and its effect on the computation of the system.
7. Display Person Count - to count the total person
8. Show Distance - The distance between individuals
9. Social Distance Threshold - To check if the distance value violates the minimum social distance set or not
10. Output will Look like

     ![image]( "Social Distancing Detection Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Social Distancing Detection
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\17 Social Distance\social distance_canteen1
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of the social distancing violated_**
     
     ![image]( "Social Distancing Detection")

***Different test Cases only for Social Distancing Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
