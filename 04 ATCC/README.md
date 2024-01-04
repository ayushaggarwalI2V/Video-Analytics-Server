# **ATCC**
 
***Steps to apply ATCC***

1. Analytic Specific Settings
   - Select Object -> car, bus. truck, bike, etc
   - Select Model
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Zones (Shown in image)
   
    ![image]( "VMS image")
   
4. Check confidence value based on the use case
5. Lane Threshold -> The total density of vehicles on the lane and setting up a threshold value for each lane
6. For Abandon Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/114)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like                                                                         
   
   ![image]( "Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. 
   - Link to video - 
   - 
   - Draw the area as shown in the image
   - Expected Output -> **_Must get alert of object_** after the stationary duration time
     
   ![image]( "")

2. 
   - Link to video - 
   - Check the background similarity factor -> Check background to use background matching algorithm for abandoned objects.
   - Expected Output -> **_Alert of the bag is generated_**
   
   ![image]( "")

3. 
   - Link to video - 
   - 
   - Check with different select objects like - cars, buses, etc
     
   ![image]( "")

4. 
   - Link to video - 
   - 
   - Check with different select objects like - cars, buses, etc
   - Expected Output -> **_No alerts are generated_** because there is no abandoned object in this video
     
   ![image]( "")

***Different test Cases only for ATCC***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
4. Check Bbox
5. Tracking of object -> ID persists, no exchange of ID
6. VA Stream Delay
7. Filter by classification objects
8. Draw Multiple zones, min-max setting
9. Check Find Attributes
10. Show tracks, trackID
11. Advance Settings
