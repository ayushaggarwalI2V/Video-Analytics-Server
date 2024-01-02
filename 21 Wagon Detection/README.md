# **Wagon Detection**
 
***Steps to apply Wagon Detection Analytic***

1. Analytic Specific Settings
   - FPS
   - Wagon counter clear time in seconds
   - Wagon Direction -> Left to Right, Right to left
   - Select text model 
2. Object Size
   - Draw Min and Max Size of the Object
4. Drawing Setting
   - Draw ROI

     ![image]( "Wagon Detection")

5. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
6. Check Frame Skipping and its effect on the computation of the system.
7. Output will Look like

     ![image]( "Wagon Detection output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Wagon Left to Right
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\21 Wagon\wagonLeftRight1
   - Draw the Min Max Object size as shown in the image
   - Must check the OCR number of the Wagon in the Alert
   - Expected Output -> **_Alert must be generated when wagon detects_**
     
     ![image]( "Wagon Detection")

2. Wagon Detection Right to Left 1
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\21 Wagon\wagonRightLeft1
   - Check the confidence value
   - Must check the OCR number of the Wagon in the Alert
   - Expected Output -> **_Alert must be generated when wagon detects_**
   
     ![image]( "Wagon Detection")

3. Wagon Detection Right to Left 2
   - Link to video - \\\192.168.1.22\Testing_team\ayush_testing_videos\21 Wagon\wagonRightLeft2
   - Check the confidence value
   - Must check the OCR number of the Wagon in the Alert
   - Expected Output -> **_Alert must be generated when wagon detects_**
   
     ![image]( "Wagon Detection")

***Different test Cases only for Wagon Detection***

1. Detection with different models
2. Check Backend -> Inference, Open CV, CUDA
3. Frame Skipping in `Analytic Advance Setting`
4. Check the confidence value in the `Analytic Specific Setting`
5. Must check the OCR number of the Wagon in the Alert
