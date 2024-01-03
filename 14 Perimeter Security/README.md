# **Perimeter Security Detection**
 
***Steps to apply Perimeter Security Detection Analytic***

1. Analytic Specific Settings
   - FPS
   - Select Object -> car, bus, person, truck, etc.
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Perimeter Line -> Make direction by right click on the arrow (allow from both directions, toggle direction)

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/14%20Perimeter%20Security/images/perimeter%20violation.png "Perimeter Security Detection")

5. Check Alert
6. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like

     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/14%20Perimeter%20Security/images/perimeter%20violation%20alert.png "Perimeter Security Detection Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Perimeter Security Detection (Crawl Video)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\14 Perimeter Counting\perimeter_person_crawl
   - Draw Perimeter Line
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of Perimeter Violation when object Cross the perimeter line_**
     
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/14%20Perimeter%20Security/images/perimeter%20violation.png "Perimeter Security Detection")

2. Perimeter Security Detection (Canteen Video)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\14 Perimeter Counting\perimeter_person1
   - Draw Perimeter line
   - Set `frame skipping` to 3 by enabling `show advance setting` 
   - Expected Output -> **_Must get alert of Perimeter Violation when object Cross the perimeter line_**
   
     ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/14%20Perimeter%20Security/images/perimeter%20violation%20inside.png "Perimeter Security Detection")

***Different test Cases only for Perimeter Security Detection***

1. Detection with different models - model1, model2...
2. Check the `backend` in analytic specific setting with OpenCV, CUDA, Inference Engine
3. Frame Skipping
4. Check with different values of confidence
5. Different values `Birth and Lost threshold` in Advance Analytic Setting 
