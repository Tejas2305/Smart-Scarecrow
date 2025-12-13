As this is my team project, we came up with the idea that the conventional scarecrows are not worth it, or they are inefficient at what they are doing. We need better ways to keep the intruders out, while still keeping it cost efficient,<br>
We sat down and discussed a few things.<br>
We found out he existing solutions for it and their key issues and the key features.<br>
We found out there are many out there that are providing the smart scarecrow solution, but we can classify them into two broader categories. First ones are the ones that are low cost but do not do the job properly, like lack multiple features and seem closer to the traditional ones. The second category is the ones that are extremely expensive, like they cost around 50000 inr to 70000inr. They have all the advanced features, but at such a high cost, the indian farmers won't adopt it.<br>
So then we discussed the features.<br>
After consideration of cost and other factors, we thought of keeping these features.<br>
1) a camera that will get the video for offline AI processing<br>
2) a low range but accurate sensor<br>
3) a long range heat sensor<br>
4) a water pump with a nozzle to shoot water when a bird or other intruders come close<br>
5) keeping it waterproof<br>
6) rain sensors with vibation from other motors(so that no dropllets remains on it which will reduce the false alarms for it<br>
7) Also, the AI will be detecting the birds and animals and based on its type, it will be using the buzzer and levels of lighting based on its type.<br>
8) We also have a moisture sensor for getting the moisture in the soil, and also other sensors to get moisture in the air( we are using this data to predict the weather too<br>
9) Keeping things simple, all the scarecrows will be covered with raincoats as waterproofing the head part, which has all the sensors, and the camera will be protected by an origami system umbrella, which will open and close using a servo motor when it rains<br>
10) During rain, the scarecrow won't function due to safety mechanisms. We will shut down all power supplies except for the rain sensor; all other parts will be shut down<br>
11) It will be working on Solar panels, and a battery, the battery will be charged by a Solar panel. In case of low charging, the battery can be swapped with a charged one, and the low-charging one can be charged at home using a power supply (for now, we are only thinking of the battery being charged using solar and not considering how they would be able to charge it at home, as its mechanism will not be designed by us right now)<br>
12) We will be using a GSM module to send the sms to the farmers (as many rural areas in India are not in coverage of the internet, like the farm area only), so we will be sending critical alerts through the sms, like intruder detected, Rain is predicted, High moisture level, camera malfunction, low battery<br>
13) main details like image of introducer and what action was taken, and will be stored in the SD card if provided, and can be taken into the app by connecting  to it using Bluetooth<br>
14) For now, we have decided to use the Raspberry Pi 3 b+ as we feel it is sufficient for our project, and it also has Bluetooth<br>



so what is done till now is <br>
a temp ai is trained with [[Link](https://universe.roboflow.com/scarecrow-skyse/merger-ax44t/model/2)]<br>
mAP@50 : 74.4%<br>
Precision : 73.3%<br>
Recall : 69.9%<br>

the above model was trained using roboflow <br>
and we also trained our own model using ai genarted code on google colab<br>
but it had poor results <br>
notebook: [Link](/file.ipynb)<br>
model details: [Link](/design_file)<br>
model file: [Link](/yolov11n_15K_run/weights/best.pt)<br>
<br>
<br>
a design is ready and below are its photos and accual files<br>
I know that the STEP file and IAM files designs are not exactly same as the dwg or they do not have all the parts which were made in dwg.<br>
as mentioned by reviewer a STEP file is mandatory but i didn't knew this thats the reason i had made a dwg file, i tried to convert it to STEP directly (using export) but that was of no use as it failed due and asked me to select some mesh(i tried to solve this error but was not able to do that) so at the end i had to make the entire design again in step files and iam.I hope that should not be any issue.
<br>
## Note for reviwer <br>
By mistake i had mentioned the project cost from an older evaluation in which the waterproof case was not considered. i kindly request you to modify this and approve my actual required budget which is currently $278.62.
I would aslo like if you can consider the real time conversion from inr to usd as the exchange rates are changing to much.
<br>
<br>
## STEP File
preview:<br>
![Crop_Cop_Final_STEP](/design_file/STEP/image.png)<br>
Video link: [Link](design_file/STEP/video.mp4)<br>
<br>
STEP Folder: [Folder link](design_file/STEP/)<br>
STEP File: [Link](design_file/STEP/lala%20hackton.STEP)<br>
Part files:<br>
[Link_1](/design_file/STEP/lala%20hackton.SLDPRT)<br>
[Link_2](/design_file/STEP/lala%20hackton2.SLDPRT)<br>
[Link_3](/design_file/STEP/lala%20hackton3.SLDPRT)<br>
[Link_4](/design_file/STEP/Part5.SLDPRT)<br>
<br>
[SLDASM File](/design_file/STEP/lala%20hackton.SLDASM)<br>
<br>
<br>
### IAM File
preview:<br>
![Crop_Cop_Final_IAM_1](/design_file/IAM/img_1.png)<br>
![Crop_Cop_Final_IAM_2](/design_file/IAM/img_2.png)<br>
<br>
IAM Folder: [Folder link](design_file/IAM/)<br>
IAM File: [Link](design_file/IAM/lala%20hackton.iam)<br>
Part files:<br>
[Link_1](/design_file/IAM/lala%20hackton.ipt)<br>
[Link_2](/design_file/IAM/lala%20hackton2.ipt)<br>
[Link_3](/design_file/IAM/lala%20hackton3.ipt)<br>
[Link_4](/design_file/IAM/Part5.ipt)<br>
<br>
<br>
### DWG Files
file: [Link](/design_file/Crop_Cop_Final.dwg)<br>
Video link: [Link](design_file/Crop_Cop_Final.mp4)<br>
preview:<br>
![Crop_Cop_Final](/design_file/Crop_Cop_Final1.png)<br>
![Crop_Cop_Final](/design_file/Crop_Cop_Final2.png)<br>
<br>
<br>
dismantled / exploded view<br>
<br>
file: [Link](/design_file/Crop_Cop_Final_2.dwg)<br>
preview:<br>
![Crop_Cop_Final_2](/design_file/Crop_Cop_Final_2.jpg)<br>
<br>
<br>
and lastly here is the estimated costs<br>
<br>
<br>
| Sr | Component | Qty | Spare | Total | Link | Cost per piece | Total cost |
|----|-----------|-----|-------|-------|------|----------------|------------|
| 1 | **Pipe 25Mm [For Spine And Leg]** | 6 | 2 | 8 | [Link](https://rebrand.ly/pipe-25mm) | ₹50.00 | ₹400.00 |
| | Leg Pipes (Ø25 × 900 Mm) | | | 0 | | | ₹0.00 |
| | Spine Pipe (Ø25 × 600 Mm) | | | 0 | | | ₹0.00 |
| | Shoulder Pipe (Ø20 × 1000 Mm) | | | 0 | | | ₹0.00 |
| | Arm Pipes (Ø20 × 450 Mm) | | | 0 | | | ₹0.00 |
| 2 | **Metal Sheet [For Head And Chest Box And Rain Flap] Kg** | 14 | 3 | 17 | [Link](https://rebrand.ly/metal-sheet) | ₹50.00 | ₹850.00 |
| | Rain Flap (350×300×3 Mm) | | | 0 | | | ₹0.00 |
| | Head Box (200×200×150 Mm) | | | 0 | | | ₹0.00 |
| | Chest Box (250×300×150 Mm) | | | 0 | | | ₹0.00 |
| 3 | **Servo Motor (Mg995/Mg996R) For Arms** | 3 | 2 | 5 | [Link](https://rebrand.ly/servo-motor) | ₹329.00 | ₹1,645.00 |
| 4 | **Solar Panel (350×250×20 Mm)** | 1 | | 1 | [Link](https://rebrand.ly/Solar-pannel) | ₹1,400.00 | ₹1,400.00 |
| 5 | **Raspberry Pi 3B+** | 1 | | 1 | [Link](https://rebrand.ly/raspberry-pi-3b-plus) | ₹4,249.00 | ₹4,249.00 |
| 6 | **Pi Camera Module Noir** | 1 | | 1 | [Link](https://rebrand.ly/raspberry-pi-camera) | ₹1,539.00 | ₹1,539.00 |
| 7 | **Pir Sensor** | 2 | 1 | 3 | [Link](https://rebrand.ly/pir-sensor) | ₹55.00 | ₹165.00 |
| 8 | **Ultrasonic Sensor (Hc-Sr04)** | 2 | 1 | 3 | [Link](https://rebrand.ly/HC-SR04) | ₹266.00 | ₹798.00 |
| 9 | **Water Spray Nozzle** | 1 | | 1 | [Link](https://rebrand.ly/sprinkler) | ₹386.00 | ₹386.00 |
| 10 | **Water Pump (12V)** | 1 | | 1 | [Link](https://rebrand.ly/water-pump) | ₹1,299.00 | ₹1,299.00 |
| 11 | **Led Strobes (Arm Ends)** | 1 | | 1 | [Link](https://rebrand.ly/LED-35c06c) | ₹399.00 | ₹399.00 |
| 12 | **Speakers (Ø40 Mm)** | 2 | | 2 | [Link](https://rebrand.ly/speaker-a) | ₹622.00 | ₹1,244.00 |
| 13 | **Gsm Module (Sim800L/Sim900)** | 1 | | 1 | [Link](https://rebrand.ly/gsm-sim800l) | ₹449.00 | ₹449.00 |
| 14 | **Solar Charge Controller (12V)** | 1 | | 1 | [Link](https://rebrand.ly/solar-controller) | ₹505.00 | ₹505.00 |
| 15 | **12V 7Ah Sla Battery** | 1 | | 1 | [Link](https://rebrand.ly/battery-12v) | ₹1,079.00 | ₹1,079.00 |
| 16 | **Buck Converters (5V)** | 1 | 1 | 2 | [Link](https://rebrand.ly/Buck-converter) | ₹169.00 | ₹338.00 |
| 17 | **Jumper Wires** | 2 | | 2 | [Link](https://rebrand.ly/Jumper-Wires-mf) | ₹88.00 | ₹176.00 |
| 18 | **Internal Wire** | 5 | 0 | 5 | [Link](https://rebrand.ly/wire-temp) | ₹15.00 | ₹75.00 |
| 19 | **Cable Zip Ties** | 1 | 0 | 1 | [Link](https://rebrand.ly/Cable-Zip-Ties) | ₹149.00 | ₹149.00 |
| 20 | **3D Printing Filament** | 2 | 0 | 2 | [Link](https://rebrand.ly/3d-printing-filament) | ₹1,270.00 | ₹2,540.00 |
| 21 | **Mounting Brackets (Servo, Nozzle, Electronics)** | As req. | 50 | 50 | NA | ₹50.00 | ₹1,000.00 |
| 22 | **Miscellaneous** | As req. | 1 | 1 | NA | ₹2,500.00 | ₹1,500.00 |
| 23 | **Waterproof Case** | 1 | 0 | 1 | [Link](https://rebrand.ly/case-waterproof) | ₹3,050.00 | ₹3,050.00 |
| | | | | | | **USD Value** | **$278.62** |
| | | | | | | **Total** | **₹25,235.00** |

*Note: USD value calculated considering 1 USD = ₹90.57.*

