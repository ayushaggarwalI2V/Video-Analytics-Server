# **Person State Detection**
 
***Steps to apply Person State Detection Analytic***
- In this analytic we detect person fallen
1. Analytic Specific Settings
   - Select Filtered Object
   - Select Object
2. Object Size
   - Draw Min and Max Size of the Object
4. Drawing Setting
   - Draw ROI

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/20%20Person%20State%20Detection/images/person%20state.png "Person State Detection")

5. For Analytic Specific Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/122)
6. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Person fallen interval -> If a person is detected as fallen, up to the configured threshold then it'll generate an event of Person_Fallen.
9. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/20%20Person%20State%20Detection/images/person%20state%20alert.png "Person State Detection output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Person State Detection Inside 
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\20 Person State Detection\fallenoffice1
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Alert must be generated when person falls_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/20%20Person%20State%20Detection/images/person%20state.png "Person State Detection")

2. Person State Detection Outside
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\20 Person State Detection\fallenOutside2
   - Check the confidence value
   - Expected Output -> **_Alert must be generated when person falls_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/20%20Person%20State%20Detection/images/person%20state%20outside2.png "Person State Detection")

3. Person State Detection (Smart City Site)
   - Link to video - 
   - Check the confidence value
   - Expected Output -> **_Alert must be generated when person falls_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/20%20Person%20State%20Detection/images/person%20state%20iocl.png "Person State Detection")

***Different test Cases only for Person State Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping in `Analytic Advance Setting`
4. Check the confidence value in the `Analytic Specific Setting`
5. No Exchange of person ID
