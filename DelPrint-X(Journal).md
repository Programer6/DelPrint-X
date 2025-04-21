Made by: @codelife / @programmer6
# 3D Printer Design: CAD & PCB Documentation

**Project Status:** Design Phase Complete (Pre-Assembly) 

**Total Design Hours:** 50 hours  💀

**CAD:** https://a360.co/43TlPJk

**Respository link:** https://github.com/Programer6/DelPrint-X

**BOM: ** https://docs.google.com/spreadsheets/u/3/d/1YkbswMdvz8Wfhi4MrrZ9T6xIMiGSr8R6hmByEVLgUXc/edit?ouid=100411957879145722379&usp=sheets_home&ths=true

Research: 5 hours
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

## Build Log

| Date         | Task                                                      | Time  | Notes                                                             |
|--------------|-----------------------------------------------------------|-------|-------------------------------------------------------------------|
| 06 Mar 2025  | BOM creation & parts sourcing                             | 8 hr  | BOM cost hit $300, so LEDs & enclosure panels were cut to budget  |
| 07 Mar 2025  | Fusion360 workspace setup & extrusion imports             | 4 hr  | Imported .dxf extrusion profiles; laid out main frame backbone     |
| 08 Mar 2025  | Hand sketches - initial CAD of frame sections              | 5 hr  | Converted rough paper sketches into base CAD geometry              |
| 09 Mar 2025  | Light CAD check-in                                        | 1 hr  | Quick session to verify slot placements after yesterday’s work     |
| 10 Mar 2025  | Detailed frame modeling: slots & cable-routing channels    | 6 hr  | Added custom slots and cable paths; heavy use of Align tool        |
| 11 Mar 2025  | NEMA 17 stepper-motor mounts                     | 5 hr  | Added them in!                 |
| 12 Mar 2025  | Quick CAD tweak: mount clearances                         | 1 hr  | Minor adjustments following test print fit checks                  |
| 13 Mar 2025  | Integrated linear rails & BMG-extruder interface          | 6 hr  | Modeled carriage interfaces and virtual bolt-up to check fit       |
| 14 Mar 2025  | Final CAD cleanup | 4 hr  |  organized folders, exported key parts        |
| 14 Mar 2025  | Wrote project journal & documentation                     | 3 hr  | Drafted this log       |

Overall, it helped me gathering references and brainstorming ideas and I also screenshot various reference images for the guides to help me out later while making my 3d printer. 

- Then made a BOM:
- 10 hours !!!!!!
- Sourced AliExpress parts:  BMG extruder, linear rails, belts. Was extremely hard to stay in budget, hit $300. Therefore I had to sctrahc of the the idea of adding LED lighting and custom enclosure panels for my 3d printer.

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
