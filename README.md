# Video-Analytics-Server
## Steps to ADD VA on VMS
1. Install Video Analytics Server Release based on operating system
2. Download the Data folder for the models
3. Check the service of Video Analytics Server
   - `In Windows` -> Open Services -> Check i2V_analytics_server service it must be running
   - `In Linux` -> sudo systemctl status i2v_analytic_server.service (service must be running)
5. Open Configuration Client in VMS
6. Open Application Tab
7. In the VA Server Add a new
8. Enter Analytics Server IP -> IP of the system in which VA is installed
9. Add ports to VMS -> To find ports check the config file in the system in which VA server is installed (Folder Structure: VA_Server -> Config -> mainConf.json)
10. Check the status of VA Server on VMS (Connected/ Dis-Connected)

## Steps to ADD VA on VMS
1. Open Configuration Client in VMS
2. Click Add
3. In Popup click `Add Devices`
4. Enter the device name according to you
5. Change Make to `Recording` and Model to `Play Recording`
6. Click `Add Selected Device`

   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/vms.png "VMS image")
   
7. Select the device you have added and add the `Stream URL` (local path of the video that you want to add)
8. Click Apply

   ![image](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/blob/main/01%20Abandon%20Object%20Detection/images/vms2.png "VMS image")
   
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
4. [ATCC (Automatic Traffic Counting And Classification)]
5. [Camera Tampering](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/05%20Camera%20Tampering)
6. [Crowd Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/06%20Crowd%20Detection)
7. [Fire Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/07%20Fire%20Detection)
8. [Face Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/08%20Face%20Detection)
9. [Garbage Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/09%20Garbage%20Detection)
10. [Intrusion Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/10%20Intrusion%20Detection)
11. [Missing Object](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/11%20Missing%20Object%20Detection)
12. [Mask Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/12%20Mask%20detection)
13. [Object Counting](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/13%20Object%20Counting)
14. [Perimeter Security](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/14%20Perimeter%20Security)
15. [Smoke Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/15%20Smoke%20Detection)
16. [Safety Gear Violation]
    * Safety Shoes
    * Safety Helmet
    * Safety vest
    * Safety Gear Violation
17. [Social Distancing Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/17%20Social%20Distancing%20Detection)
18. [VIDS]
19. [Weapon Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/19%20Weapon%20Detection)
20. [Person State Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/20%20Person%20State%20Detection)
21. [Wagon Detection](https://github.com/ayushaggarwalI2V/Video-Analytics-Server/tree/main/21%20Wagon%20Detection)
