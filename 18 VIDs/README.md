# **VIDS Detection**
 
***Steps to apply VIDS Analytic***

1. In Vids Analytics we detect
   - Human Detection
   - Acceleration of vehicle (for the given threshold)
   - Deacceleration of vehicle (for the given threshold)
   - Stop Vehicle
   - Detects Illegal Vehicle (Select from Analytic Specific Setting)
   - Reverse Direction of Vehicle (Enter Valid Direction by clicking on individual `wrongDirectionArea` in `Drawing Setting`)
   - State of Traffic like Congested, Heavy Traffic
2. Analytic Specific Settings
   - Select Object
   - Check Stationary Duration Time                                 
   - Check Filter by Classification - To get alerts of only Selected items
3. Object Sizes
   - Draw Min and Max Size of the Object
4. Drawing Setting
   - Draw ROI
   - Draw Safe line (Shown in the image)
   - Draw Zones (Shown in image) -> We can make multiple zones as per requirement
   - Select Zone for the detection of multiple analytics like - Human detection, Acceleration, de-acceleration, Illegal vehicle, etc.
   
    ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/images/vids.png "VMS image")
   
5. Check Alert When violates the rules
6. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. For More information on VIDS [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/128)
9. Check Frame Skipping and its effect on the computation of the system.
10. Output will Look like
   - #### Acceleration Detection
      
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/images/accelerated.png "Output")
   
   - #### Deacceleration Detected
      
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/images/deaccelerated.png "Output")

   - #### Human Detection
      
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/images/human%20detect.png "Output")

   - #### Illegal Vehicle

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/images/illlegal.png "Illegal Vehicle")

   - #### Vehicle Stopped

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/images/stop%20vehicle.png "stop vehicle")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Highway Scenario
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\18 VIDs\acceleration_highway1
   - Draw Safe line
   - Draw wrong way direction area
   - In Illegal Vehicle select truck
   - Select Valid Direction as `Down to Top`
   - Select the Area then select analytics -> Acceleration, Deacceleration, Illegal Vehicle, Reverse direction
   - Expected Output -> **_Must get an alert of the object when it violates the given conditions_**
     
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/images/vids.png "Highway Scenario")

2. Stop Vehicle Detection 
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\18 VIDs\illegalVehicle_highway2
   - Enable ` Check Stop Vehicle` in the Select Shape property of wrongDrirectionArea
   - Also we can test multiple detections based on videos
   - Expected Output -> **_Alert of the stop vehicle is generated when the vehicle stops inside the zone_**
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/images/stop%20.png "stop vehicle")

#### Check more videos of VIDS on (\\192.168.1.22\Testing_team\ayush_testing_videos\18 VIDs) and apply analytics based on the use case and video type of analytic

***Different test Cases only for Abandon***

1. Check individual analytic detection 
2. Detection with different models
3. Check Backend -> Inference, Open CV, CUDA
4. Frame Skipping
5. Check Bbox
6. Tracking of object -> ID persists, no exchange of ID
7. VA Stream Delay
8. Safe Distance Line Violation
9. Mulitple analytics and its count
10. Draw Multiple zones, min-max setting
11. Check Find Attributes
12. Show tracks, trackID
13. Advance Settings

