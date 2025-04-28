Made by: @codelife / @programmer6
# 3D Printer Design: CAD & PCB Documentation

**Project Status:** Design Phase Complete (Pre-Assembly) 

**Total Design Hours:** 50 hours  💀

**CAD:** https://a360.co/43TlPJk

**Respository link:** https://github.com/Programer6/DelPrint-X

**BOM:** https://docs.google.com/spreadsheets/u/3/d/1YkbswMdvz8Wfhi4MrrZ9T6xIMiGSr8R6hmByEVLgUXc/edit?ouid=100411957879145722379&usp=sheets_home&ths=true

## Project Overview

Del-X is a custom‑designed 3dprinter, fully OPEN Source.  
This build was my deep dive into printer mechanics, electronics, and is open‑source project you can replicate or remix made for [Infill](https://infill.hackclub.com).


- **Print Volume:** 220 × 220 × 250 mm  
- **Frame:** 2020 & 2040 aluminum extrusion  
- **Motion:** CoreXY with linear rails  
- **Electronics:** SKR Mini E3 V2.0 & TMC2209 drivers


| Date         | Task                                                      | Time  | Notes                                                             |
|--------------|-----------------------------------------------------------|-------|-------------------------------------------------------------------|
| 06 Mar 2025  | BOM creation & parts sourcing                             | 10 hr  | Spent the  multiple days listing all required components—frame, motors, electronics, fasteners. Initial BOM cost hit $300, so I revised it by cutting back on high-density LEDs and replacing acrylic panels with MDF for the enclosure. This part mainly took so long a I had to search of the cheapest other then that I also had to orgaize information into Parts	Qty Needed	Pkg Qty	Order Qty	Cost	Link (see image below. ) to avoid over/under-ordering <img width="1310" alt="Screenshot 2025-04-03 at 3 00 45 PM" src="https://github.com/user-attachments/assets/784aba21-2c1b-4688-89b6-0174172d6d68" />|
| 07 Mar 2025  | Fusion360 workspace setup & extrusion imports             | 4 hr  | Imported .dxf extrusion profiles; create the extrustion in the correct size out main frame backbone <br> <img width="421" alt="Screenshot 2025-04-03 at 3 16 59 PM" src="https://github.com/user-attachments/assets/67fa16bd-d5fe-4cbe-9f61-692940f863a8" />   |
| 08 Mar 2025  | Hand sketches - initial CAD of frame sections              | 5 hr  | Converted rough paper sketches (see below ) this really helped to see where each extrusion goes! and actually placed them in the correct positions!      <br> ![78cf1d24-5fae-4f19-996d-61075a653ac4](https://github.com/user-attachments/assets/07696474-5d67-4736-bfbd-87349bee86ec)      |
| 09 Mar 2025  | Light CAD check-in                                        | 1 hr  | Quick session to verify slot placements after yesterday’s work once they where all right modeled a slots for T-nuts   |
| 10 Mar 2025  | Detailed frame modeling: slots & cable-routing channels    | 6 hr  | Added custom slots and cable paths; heavy use of Align tool on fusion360 to make sure that everything fit perfectly!      |
| 11 Mar 2025  | NEMA 17 stepper-motor mounts                     | 5 hr  | Added them in and making sure they had clearance for wires and matched mounting hole specs                |
| 12 Mar 2025  | Quick CAD tweak: mount clearances                         | 1 hr  | Minor adjustments following test print fit checks                  |
| 12 Mar 2025  | Desgined PCB                      | 3 hr  | Laid out the 10×10 NeoPixel matrix in KiCad which is going to be controlled using the ESP32. also added it mic so that I can make a music reative animation while not in use  (showing prionter progress)                |
| 14 Mar 2025  | Final CAD cleanup | 4 hr  |  Organized all Fusion360 folders into a logically. Exported key frame and mount parts as STEP so that I can easily find them during the time of 3D printing and anmed every component properly..       |
| 14 Mar 2025  | Wrote project journal & documentation                     | 3 hr  | Wrote logs for each day’s progress which you are reading rn.      |



## Research: 10 hours
I am completely inexperienced in 3D printing (I don't even have one 🥲 like not even a cheapo one 😅) so obviously spent a good amount of time (way too much) researching how it works! The maker mash-up tutorial seemed quite detailed and helpful.
<img width="1271" alt="Screenshot 2025-04-03 at 2 55 19 PM" src="https://github.com/user-attachments/assets/37b0918d-4e6c-4ec2-b78b-2466a5aa6df0" />

Here is some research that I did after reviwing AK printer'S documentation which came in clutch:

- https://www.instructables.com/How-to-Design-and-Build-a-3D-Printer/
- https://kingroon.com/blogs/3d-print-101/cartesian-vs-corexy
- https://reprap.org/wiki/Build_A_RepRap
- https://www.instructables.com/Complete-newbie-step-by-step-3D-printer-with-all-p/
- https://www.drdflo.com/pages/Guides/How-to-Build-a-3D-Printer/FFF.html
- https://www.geeky-gadgets.com/mondrian-customisable-reprap-3d-printer-07-12-2015/
- https://reprap.org/wiki/Choosing_a_Power_Supply_for_your_RepRap

  Overall, it helped me gathering references and brainstorming ideas and I also screenshot various reference images for the guides to help me out later while making my 3d printer. 

## Build Log



- Then made a BOM:
- 10 hours !!!!!!
- Sourced AliExpress parts:  BMG extruder, linear rails, belts. Was extremely hard to stay in budget, hit $300. Therefore I had to sctrahc of the the idea of adding LED lighting and custom enclosure panels for my 3d printer.

## 📦 Bill of Materials

| Part                                               | Qty Needed           |
|----------------------------------------------------|----------------------|
| 40×40 mm aluminum extrusion (400 mm long)           | 2                    |
| 20×20 mm aluminum extrusion (400 mm long)           | 1                    |
| 20×20 mm aluminum extrusion (190 mm long)           | 1                    |
| 20×20 mm aluminum extrusion (220 mm long)           | 2                    |
| 20×40 mm aluminum extrusion (400 mm long)           | 4                    |
| 2020 corner brackets                                | 6                    |
| Bed springs                                        | 4                    |
| 8 mm linear rods (400 mm long)                     | 4                    |
| 8 mm linear rods (440 mm long)                     | 2                    |
| Jumper wires                                       | 6                    |
| Endstop (limit) switches                           | 3                    |
| M5 × 8 mm socket‑cap screws                        | 100                  |
| MK2B heated bed (214 mm square)                    | 1                    |
| E3D V6 hotend with heater (24 V) + thermistor       | 1                    |
| SKR Mini E3 V2.0 mainboard + TMC2208 drivers        | 1                    |
| 360 W power supply (24 V)                          | 1                    |
| 5015 blower fan (24 V)                             | 1                    |
| 40 mm muffin fan (24 V)                            | 1                    |
| Redrex dual‑drive BMG Bowden extruder              | 1                    |
| NEMA 17 stepper motors                             | 5                    |
| Glass print surface (214 mm square)                | 1                    |
| Corner braces                                      | 8                    |
| M3/M4/M5 screw assortment (various sizes)           | Assortment           |
| GT2 timing belt + pulleys                           | 1 kit                |
| 625 2RS ball bearings (5 × 16 × 5 mm)               | 6                    |
| Lead screws (8 mm × 295 mm) with nuts               | 2                    |
| M3/M4/M5 T‑nuts (various)                          | Assortment           |
| Spiral cable wrap                                   | 4 m                 |
| Zip ties                                            | 20                   |
| Power cable                                         | 1                    |
| Power switch                                        | 1                    |
| Washer assortment (mixed sizes)                     | Assortment           |
| Idler pulley                                        | 1                    |
| Silicone insulated wire (16 AWG)                    | 2 m                 |
| 12864 LCD Smart Controller (graphical display)      | 1                    |

---

[FUll BOM link](https://docs.google.com/spreadsheets/d/1YkbswMdvz8Wfhi4MrrZ9T6xIMiGSr8R6hmByEVLgUXc/edit?gid=0)


<img width="1310" alt="Screenshot 2025-04-03 at 3 00 45 PM" src="https://github.com/user-attachments/assets/784aba21-2c1b-4688-89b6-0174172d6d68" />

After most of the parts where sourced I worked on getting a bit of underdstanding on how the 3d printer is actually supposed to be put together before actually doing by making sketch (really rough - yes, I know my handwrithing is horrible). 

![78cf1d24-5fae-4f19-996d-61075a653ac4](https://github.com/user-attachments/assets/07696474-5d67-4736-bfbd-87349bee86ec)

Making of the cad:

<img width="421" alt="Screenshot 2025-04-03 at 3 16 59 PM" src="https://github.com/user-attachments/assets/67fa16bd-d5fe-4cbe-9f61-692940f863a8" />


Getting organized was the first step. I created a new project workspace in Fusion360. For the extursion, cad parts, etx. I designed them in a different fusion360 file and then added then in to the main file. Slowly bring my hand-drawn sketches into alive!
The frame is the backbone of the printer (Frame = backbone = MUST be solid.), so I invested significant time. Luckly I didn't need to design them from scratch as I was able to download the exturstion in the .dfx format and then adjust it too my size whihch helped me save some time in the desiging process.


- Slowly I progressed my way through added custom mounting features such as slots. Used the fusions360 align feature to make sure the fitted perfectly.
- Then progressed with adding NEMA 17 stepper motors on the its mounts
---


<img width="551" alt="Screenshot 2025-04-03 at 3 18 47 PM" src="https://github.com/user-attachments/assets/faa5f416-5246-42e2-a225-82c5f8999c0c" />
<img width="533" alt="Screenshot 2025-04-03 at 3 19 25 PM" src="https://github.com/user-attachments/assets/4180f5a9-9add-4d90-9d14-73292d939ec5" />



# Making of the 3D printer 

Image of which so the the different size of extrusion and once up together!
<br>

<img width="357" alt="Screenshot 2025-04-23 at 5 37 09 PM" src="https://github.com/user-attachments/assets/921faed7-f6b6-493a-987e-0586451407f6" />
<img width="522" alt="Screenshot 2025-04-23 at 5 36 33 PM" src="https://github.com/user-attachments/assets/a6475538-f0ff-4fe6-9099-2f127849088d" />

Imag of adding the slots in!

<br>
<img width="680" alt="Screenshot 2025-04-23 at 5 42 02 PM" src="https://github.com/user-attachments/assets/f63b8326-56dc-4eab-a103-f9efabda319b" />

More images!
<br>
<img width="470" alt="Screenshot 2025-04-23 at 5 43 56 PM" src="https://github.com/user-attachments/assets/a0749810-7c50-4431-a4da-18d394e89bd1" />
<img width="786" alt="Screenshot 2025-04-23 at 5 46 48 PM" src="https://github.com/user-attachments/assets/2cdcee86-d86e-47be-b08a-5ee63577dd69" />



# Other Cool Ideas I have!
I’ll planning to use ESP-EYE module (I already have this - will ask from my coding teacher) to monitor my 3D printer in real time. Since the ESP-EYE has a built-in camera and WiFi, I’ll flash it with a video streaming firmware which I will code and mount it near the printer to watch the print bed remotely (Via eg. youtube). If i have engouh time I am also think of experimenting with the ESP-EYE’s AI features to detect motion and hopefully dectect fails in order to create a system in which it will send me a SMS. 

For my PCB was thinking use to use my custom 10×10 NeoPixel board which I designed through Pixeldust (yay! no need to add to BOM) to show the progress percentage of my 3D prints. The idea is to light up the LEDs row by row based on how much of the print is done—like each pixel represents 1%, so when it hits 100%, the whole grid lights up.
<img width="526" alt="Screenshot 2025-04-23 at 4 44 20 PM" src="https://github.com/user-attachments/assets/7df78473-2954-476d-bcfd-11adae5097c4" />
<img width="953" alt="Screenshot 2025-04-23 at 4 44 37 PM" src="https://github.com/user-attachments/assets/5dbf088a-69a1-4953-8ca0-5ac58bb13940" />


