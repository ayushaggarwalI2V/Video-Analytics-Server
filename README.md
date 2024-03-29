# Video-Analytics-Server
## Steps to Add VA on VMS
1. Install Video Analytics Server Release based on operating system
2. Download the Data folder for the models
3. Check the service of Video Analytics Server
   - `In Windows` -> Open Services -> Check i2V_analytics_server service it must be running
   - `In Linux` -> Use below command to check the status of service (service must be running)
```
    sudo systemctl status i2v_analytic_server.service
```
4. VA Server service must be running
5. Open Configuration Client in VMS
6. Open Application Tab
7. In the VA Server Add a new
8. Enter Analytics Server IP -> IP of the system in which VA is installed
9. Add ports to VMS -> To find ports check the config file in the system in which VA server is installed
   - (Folder Structure: VA_Server -> Config -> mainConf.json)
11. Check the status of VA Server on VMS (Connected/ Dis-Connected)

## Steps to Add Devices for VA on VMS
1. Open Configuration Client in VMS
2. Click Add (only for testing video)
3. In Popup click `Add Devices`
4. Enter the device name according to you
5. Change Make to `Recording` and Model to `Play Recording`
6. Click `Add Selected Device`

   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/vms.png "VMS image")
   
7. Select the device you have added and add the `Stream URL` (local path of the video that you want to add)
8. Click Apply

   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/vms2.png "VMS image")

9. Go to the `Application` tab in VMS
10. Select VA server
11. Click `Select Camera` -> Then from the device list Select the camera in which you want to apply analytics
12. Click Apply

   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/va.png "VMS image")
   
## Steps to Apply VA on VMS
1. Open `Live View Client`
2. Open the device in the view
3. Right-click on the video
4. Select `Apply Video Analytics`

   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/lv.png "VMS image")
   
5. For Every analytics check below references
   
## List of Analytics
1. [Abandon Object](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/01%20Abandon%20Object%20Detection)
2. [Advance Motion Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/02%20Advance%20Motion)
3. [Action Recognition](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/03%20Action%20Recognition)
   * Fight Detection
   * Waving Detection
5. [ATCC (Automatic Traffic Counting And Classification)]()
6. [Camera Tampering](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/05%20Camera%20Tampering)
7. [Crowd Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/06%20Crowd%20Detection)
8. [Fire Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/07%20Fire%20Detection)
9. [Face Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/08%20Face%20Detection)
10. [Garbage Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/09%20Garbage%20Detection)
11. [Intrusion Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/10%20Intrusion%20Detection)
12. [Missing Object](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/11%20Missing%20Object%20Detection)
13. [Mask Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/12%20Mask%20detection)
14. [Object Counting](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/13%20Object%20Counting)
15. [Perimeter Security](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/14%20Perimeter%20Security)
16. [Smoke Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/15%20Smoke%20Detection)
17. [Safety Gear Violation](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/README.md)
    * [Safety Helmet](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/README.md#no-helmet-inside)
    * [Safety shoes](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/README.md#no-shoes-iocl)
    * [Safety vest](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/README.md#no-safety-vest)
    * [Safety shoes and helmet](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/16%20Safety%20Gear%20Violation/README.md#no-helmet-and-no-vest-outside)
18. [Social Distancing Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/17%20Social%20Distancing%20Detection)
19. [VIDS](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/18%20VIDs)
    * [Acceleration Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/README.md#acceleration-detection)
    * [Deacceleration Detected](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/README.md#deacceleration-detected)
    * [Human Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/README.md#human-detection)
    * [Illegal Vehicle](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/README.md#illegal-vehicle)
    * [Vehicle Stopped](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/18%20VIDs/README.md#vehicle-stopped)
20. [Weapon Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/19%20Weapon%20Detection)
21. [Person State Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/20%20Person%20State%20Detection)
22. [Wagon Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/21%20Wagon%20Detection)

## Important Points to be Remember for VA Server
1. At a time only 1 VA server is attached to only 1 Application
2. To Create multiple VA servers have to create multiple services of VA [Check This to create multiple services](https://stackoverflowteams.com/c/i2v-systems/questions/140)
3. Then Add the new VA to VMS
 
## VA Basic API Calls
1. To Check the version of VA ->
   - http://(IP of system in which va is installed):(rest port)/analytic/version
   - eg-> http://192.168.1.161:5018/analytic/version
2. To Check the status of running analytics and details ->
   - http://(IP of system in which va is installed):(rest port)/analytic/details
   - eg-> http://192.168.1.161:5018/analytic/status
3. To Check the VA stream in the browser ->
   - http://(ip):(streaming port)/(cameraId)_(cameraName)_basic
   - eg-> http://192.168.1.161:8093/128_atcc_city_oneWay1_basic

## Basic Troubleshooting Steps
1. If VMS shows VA is not connected then Check the Analytic Server port in config json and check the status of the service
2. If the service not starting check port whether it is acquired by another program
3. Alerts not coming - check alert sending port
4. VA Stream not coming - check streaming port
5. Service does not start and shows `unable to find the path or recursive error` in Linux then delete the `logs` folder in the VA server folder
6. Error -> `Unable to load weight file` then the model is missing in the data folder
   - Path of data folder
   - for windows -> C:\Program Files (x86)\I2V\VA_Server
   - for linux -> opt/i2v-analytic-server/analytic_server
7. VA Models \\192.168.1.22\Testing_team\ayush_testing_videos\va_data_models)
