# **ATCC (Automatic Traffic Counting And Classification)**
 
***Steps to apply ATCC***

1. Analytic Specific Settings
   - Select Object -> car, bus. truck, bike, etc
   - Select Model
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Zones (Shown in image)
   
    ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/04%20ATCC/images/atcc_city.png "VMS image")
   
4. Check confidence value based on the use case
5. Lane Threshold -> The total density of vehicles on the lane and setting up a threshold value for each lane
6. For Advance Analytic Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like                                                                         
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/04%20ATCC/images/alert%20atcc.png "Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. ATCC City
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\04 ATCC\atcc_city_oneWay1
   - Draw the area as shown in the image
   - Check the total object count and individual object count
   - Expected Output -> **_Must get alert of ATCC_** 
     
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/04%20ATCC/images/atcc_city.png "city")

2. ATCC Tunnel
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\04 ATCC\atcc_tunnel3
   - In select object setting from the `Analytic Specific Setting` select car only
   - Check only the alert of the car is shown
   - Draw 1 lane and check to count the object
   - Expected Output -> **_Alert of ATCC object_**
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/04%20ATCC/images/atcc%20tunnel.png "tunnel")

3. ATCC Highway
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\04 ATCC\atcc_highway5
   - Draw multiple lanes and check individual lane count
   - Check with different select objects like - cars, buses, etc
   - Expected Output -> **_Alert of ATCC object_**
     
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/04%20ATCC/images/atcc%20highway.png "highway")

***Different test Cases only for ATCC***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
4. Check Bbox
5. Tracking of object -> ID persists, no exchange of ID
6. VA Stream Delay
7. Check the count of individual objects
8. Draw Multiple lanes, min-max setting
9. Check Find Attributes
10. Show tracks, trackID
11. Advance Settings
