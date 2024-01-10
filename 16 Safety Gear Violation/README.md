# **Safety Gear Violation**
 
***Steps to apply Safety Gear Analytic***

1. Analytic Specific Settings
   - Select Object -> person
   - Select Default Model for basic purposes like -> detecting persons and basic objects
   - In Safety Gear Analytic we detect -> Safety Helmets, Safety Vests, Safety Shoes, Safety Mask
   - For Each detection, we select models and their backend
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Zones (Shown in image)
   
    ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/images/safety%20gear%20violation.png "VMS image")

4. Confidence -> 0 to 1 value { Detected object confidence like 1 means fully confident 0 means least confident }
5. Save Image -> to save the analytic image
6. Max Classification - Total Number of persons in which VA process analytic
7. Selected shape properties:- In shape properties, we can change zone-wise properties like zone name stroke width and color
8. For Analytic Specific Setting of Safety Gear Violation [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/130)
9. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
10. Check Frame Skipping and its effect on the computation of the system.
11. Output will Look like
   - Safety Helmet
      
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/images/safety%20helmet.png "Output")
   
   - Safety Shoes
      
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/images/safety%20shoes%20alert.png "Output")

   - Safety Vest
      
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/images/safety%20vest.png "Output")
   
***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. No Helmet Inside
   - \\192.168.1.22\Testing_team\ayush_testing_videos\16 Safety Gear Violation\noHelmet_inside_iocl5
   - Enable the `detect no helmet` check in the analytic-specific setting
   - Check detection on different models
   - Draw the area as shown in the image
   - Expected Output -> **_Must get alert of Safety Gear Violation of no helmet_** when person has no helmet
     
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/images/safety%20gear%20violation.png "zone")

2. No Shoes IOCL
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\16 Safety Gear Violation\noShoes_iocl1
   - Enable the `detect no safetyshoes` check in the analytic-specific setting
   - Draw the area as shown in the image
   - Expected Output -> **__Must get alert of Safety Gear Violation of no shoes_** when person has no safety shoes
   
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/images/no%20shoes.png "zone")

3. No Safety Vest
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\16 Safety Gear Violation\noVest_city2
   - Enable the `detect no safety vest` check in the analytic-specific setting
   - Draw the area as shown in the image
   - Expected Output -> **_Must get alert of Safety Gear Violation of no safety vest** when the person has no vest
     
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/images/no%20vest%20vms.png "zone")

4. No Helmet and No Vest Outside
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\16 Safety Gear Violation\noHelmet_outside3
   - In Select Object choose face, person
   - Enable the `detect no helmet` and `detect no safety vest` checks in the analytic-specific setting
   - Draw the area as shown in the image
   - Expected Output -> **_Must get alert of Safety Gear Violation of no helmet_** when person has no helmet and no safety vest
     
   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/images/helmet%20and%20vest.png "zone")

***Different test Cases only for Safety Gear Violation***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping
4. Check Bbox
5. Tracking of object -> ID persists, no exchange of ID
6. VA Stream Delay
7. Multiple Detection
8. Draw Multiple zones, min-max setting
9. Check Find Attributes
10. Show tracks, trackID
11. Impact of model height and processing height

