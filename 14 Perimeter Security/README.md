# **Perimeter Security Detection**
 
***Steps to apply Perimeter Security Detection Analytic***

1. Analytic Specific Settings
   - FPS
   - Select Object -> head, face
2. Object Sizes
   - Draw Min and Max Size of the Object
3. Drawing Setting
   - Draw ROI
   - Draw Zone

     ![image]( "Perimeter Security Detection")

5. Check Alert
6. For Advance Setting [Check This](https://stackoverflowteams.com/c/i2v-systems/questions/132)
7. Check Frame Skipping and its effect on the computation of the system.
8. Output will Look like

     ![image]( "Perimeter Security Detection Output")

***Different test Cases for different videos***
##### Find Videos on _\\192.168.1.22\Testing_team\ayush_testing_videos_

1. Perimeter Security Detection (Crawl Video)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\14 Perimeter Counting\perimeter_person_crawl
   - Draw zone
   - Draw the Min Max Object size as shown in the image
   - Expected Output -> **_Must get alert of no mask face_**
     
     ![image]( "Perimeter Security Detection")

2. Perimeter Security Detection (Canteen Video)
   - Link to video - \\192.168.1.22\Testing_team\ayush_testing_videos\14 Perimeter Counting\perimeter_person1
   - Set `frame skipping` to 3 by enabling `show advance setting` 
   - Expected Output -> **_Must get alert of no mask face_**
   
     ![image]("Perimeter Security Detection")

***Different test Cases only for Perimeter Security Detection***

1. Detection with face different models - face1, face2 ...
2. Detection with different Mask Classification Model
3. Frame Skipping
4. Check with different value of confidence
5. Different values `Birth and Lost thresold` in Advance Analytic Setting 
