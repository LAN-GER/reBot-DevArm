# 🤖 reBot DevArm Open Source Hardware Specification


<p align="center">
  <img src="../../media/RS5_56.png" alt="reBot-DevArm Banner">
</p>
<p align="center">
  <strong>
    <a href="./README_zh.md">简体中文</a> &nbsp;|&nbsp;
    <a href="./README.md">English</a> &nbsp;|&nbsp;
    <a href="./README_fr.md">français</a>&nbsp;|&nbsp;
    <a href="./README_es.md">Español</a>
  </strong>
</p>


| Date | Version | File Name | Changelog |
|----------|------|----------|------|
|  2026-07-09 | v1.0 |  reBot_B601_RS_v1.0_20260625.step  | Initial upload |


This BOM is for the reBot Arm B601 RS robotic arm, which uses ROBOSTRIDE series motors. The other version, reBot Arm B601 DM, uses DAMIAO motors; [see the BOM here](../reBot_B601_DM/readme.md).

# 📦 File Structure
*   3D_Printed_Parts/: Step files for all 3D printed parts.
*   Metal_Parts/: Step files for all CNC machined metal parts.
*   Purchased_Parts/: Step files for all purchased components.
*   reBot_B601_RS_v1.0_20260625.step: Full robotic arm assembly file.

# 🛒[Gets All Parts](https://www.seeedstudio.com/reBot-Arm-B601-RS-Disassembly-Kit-Version-with-Power-Supply-Bundle.html)
- We offer five kit options:
  - **reBot-Arm-B601-RS-Disassembly-Kit**
  - **reBot-Arm-B601-RS-Assembly-Version**

# 📊 Bill of Materials (BOM)

> [!WARNING]
> Declaration: The published BOM does **not** represent the final shipping version from Seeed. This open-source v1.0 is optimized for developers to reproduce at minimal cost, with some non-essential details simplified.
> The final Seeed production version will include metal laser engraving for foolproofing, some 3D printed parts will be replaced with metal for durability, clearances and machining tolerances will be adjusted for factory variation (balancing precision and cost), and custom wiring (e.g., braided sleeve protection) will be added at extra cost. However, the mechanical structure remains identical.

---

## 🖨️ 3D Printed Parts

| Part Description | Image | File Name | Material | Qty | Notes |
|----------|------|--------|------|----------|------|
| Robotic Arm Base Platform | <img src="./3D_Printed_Parts/images/02-BASE.png" width="80"> | 1-BASE-PLATE.step | Bambu ABS Black | 1 | 0.4 nozzle, 0.2 layer height, 30% infill |
| Robotic Arm Base Link | <img src="./3D_Printed_Parts/images/02-BASE_02.png" width="80"> | 1-RSM1-STATOR-1.step | Bambu ABS Black | 1 | 0.4 nozzle, 0.2 layer height, 30% infill |
| Upper Arm Left Filler | <img src="./3D_Printed_Parts/images/02-DOWN_TRIM_1.png" width="80"> | 1-DOWN-DL.step | Bambu PLA Black & Green | 1 | 0.4 nozzle, 0.2 layer height, 15% infill |
| Upper Arm Right Filler | <img src="./3D_Printed_Parts/images/02-DOWN_TRIM_2.png" width="80"> | 1-DOWN-DR.step | Bambu PLA Black & Green | 1 | 0.4 nozzle, 0.2 layer height, 15% infill |
| Upper Arm and Lower Arm Center Filler | <img src="./3D_Printed_Parts/images/02-DOWN-FILLING.png" width="80"> | 1-SPACE-UP.step | Bambu ABS Black | 2 | 0.4 nozzle, 0.2 layer height, 30% infill |
| Arm Handle | <img src="./3D_Printed_Parts/images/02-HANDLE.png" width="80"> | 1-HANDLE.step | Bambu ABS Black | 1 | 0.4 nozzle, 0.2 layer height, 30% infill |
| Upper and Lower Arm Cover | <img src="./3D_Printed_Parts/images/02-DOWN-COVER.png" width="80"> | 1-COVER.step | Bambu PLA Green | 2 | 0.4 nozzle, 0.2 layer height, 15% infill |
| Lower Arm Left Filler | <img src="./3D_Printed_Parts/images/02-UP-TRIM_1.png" width="80"> | 1-UP-DL.step | Bambu PLA Black & Green | 1 | 0.4 nozzle, 0.2 layer height, 15% infill |
| Lower Arm Right Filler | <img src="./3D_Printed_Parts/images/02-UP-TRIM_2.png" width="80"> | 1-UP-DR.step | Bambu PLA Black & Green | 1 | 0.4 nozzle, 0.2 layer height, 15% infill |
| Gripper Horizontal Limit | <img src="./3D_Printed_Parts/images/02-SPACER.png" width="80"> | 1-STOPPER-1.step | Bambu PLA Green | 1 | 0.4 nozzle, 0.2 layer height, 15% infill |
| Gripper Slider Support Bracket | <img src="./3D_Printed_Parts/images/02-3D-RAIL-BRACKET.png" width="80"> | 1-RAIL-BASE-2.step | Bambu PLA Green | 1 | 0.4 nozzle, 0.2 layer height, 15% infill |
| Gripper Finger | <img src="./3D_Printed_Parts/images/02-CLIP_1.png" width="80"> | 1-CLIP.step | Bambu ABS Black | 2 | 0.4 nozzle, 0.2 layer height, 45% infill. Print from the side of the gripper to improve its structural strength. |


Long-term dragging of Wiring Harness 1 may abrade the motor connector and result in poor electrical contact. Printing the parts listed below can mitigate this risk.

| Part Description | Image | File Name | Material | Qty | Remarks |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Wiring Harness Clips for Two Sides of Motor 1 | <img src="./3D_Printed_Parts/images/RS_Motor1_wiring_harness_clip.jpg" width="80"> | `RS_Motor1_wiring_harness_clip.stp` | Bambu Lab Black ABS | 2 | 0.4 mm nozzle, 0.2 mm layer height, 30% infill |

### 🧩 Printing Recommendations
- Layer height: 0.2 mm
- Nozzle: 0.4 mm
- Supports: Add as needed
- Materials: High-temperature and load-bearing parts use ABS with 30–80% infill; may also use nylon or carbon-fiber reinforced materials. Cosmetic parts use PLA with 15% infill.
- Recommended materials for load-bearing parts:

---

## 🔩 CNC Machined Metal Parts

> [!WARNING]
> Some parts that can be replaced with 3D printing are noted in the remarks, which can significantly reduce costs.

| Part Description | Image | File Name | Material | Qty | Machining | Notes |
|----------|------|--------|----------|------|------|------|
| Motor 1 Bearing Mount | <img src="./Metal_Parts/images/02_Base_Reinforcement_Part.png" width="80"> | 2-RSM1-ROTOR-1.step | Aluminum Alloy 5052 | 1 | CNC |  |
| Link1 Left Metal | <img src="./Metal_Parts/images/Link1_Left_Metal.png" width="80"> | 2-RSM-ROTOR-L.step | Aluminum Alloy 5052 | 1 | CNC |  |
| Link1 Right Metal | <img src="./Metal_Parts/images/Link1_Right_Metal.png" width="80"> | 2-RSM-ROTOR-R.step | Aluminum Alloy 5052 | 4 | CNC ||
| Link1 Bottom Metal | <img src="./Metal_Parts/images/Link1_Bottom_Metal.png" width="80"> | 2-RSM1-ROTOR-1.step | Aluminum Alloy 5052 | 3 | CNC | |
| Joint Metal Disc  | <img src="./Metal_Parts/images/2-CD.png" width="80"> | 2-CD.step | Aluminum Alloy 5052 | 3 | CNC | Used to Conceal Screws |
| RS06 Front Extesnion | <img src="./Metal_Parts/images/RS06_Front_Extesnion.png" width="80"> | 2-RSM2-STATOR-1.step | Aluminum Alloy 5052 | 2 | CNC | |
| RS06 Back Extesnion | <img src="./Metal_Parts/images/RS06_Back_Extesnion.png" width="80"> | 2-RSM2-STATOR-2.step | Aluminum Alloy 5052 | 2 | CNC | |
| Link2 Left and Right Metal | <img src="./Metal_Parts/images/2-LINK-2_3.png" width="80"> | 2-LINK-2_3.step | Aluminum Alloy 5052 | 2 | CNC | |
| Upper Limit L | <img src="./Metal_Parts/images/Upper_limit_L.png" width="80"> | 2-Upper-Limit_L.stp | Aluminum Alloy 5052 | 1 | CNC | |
| Upper Limit R | <img src="./Metal_Parts/images/Upper_limit_R.png" width="80"> | 2-Upper-Limit_R.stp | Aluminum Alloy 5052 | 1 | CNC | |
| Lower & Upper Link L| <img src="./Metal_Parts/images/2-RSM3-ROTATOR-L.png" width="80"> | 2-RSM3-ROTATOR-L.step | Aluminum Alloy 5052 | 1 | CNC | |
| Lower & Upper Link R| <img src="./Metal_Parts/images/2-RSM3-ROTATOR-R.png" width="80"> | 2-RSM3-ROTATOR-R.step | Aluminum Alloy 5052 | 1 | CNC | |
| Link3 Left Metal| <img src="./Metal_Parts/images/Link3-Left-Metal.png" width="80"> | 2-LINK-3_4-L.step | Aluminum Alloy 5052 | 1 | CNC | |
| Link3 Right Metal| <img src="./Metal_Parts/images/Link3-Right-Metal.png" width="80"> | 2-LINK-3_4-R.step | Aluminum Alloy 5052 | 1 | CNC | |
| Link3 Right & Left Link | <img src="./Metal_Parts/images/Link3-Right-Left-Link.png" width="80"> | 2-SPACE-UP-2.step | Aluminum Alloy 5052 | 1 | CNC | |
| Motor4-7 Cable Fixing | <img src="./Metal_Parts/images/Motor4_Cable_Fixing.png" width="80"> | 1-O-CLIP.step | Aluminum Alloy 5052 | 4 | CNC | Seeedstudio ships this part as a single CNC-machined metal component integrated with another part, which drives up manufacturing costs. If you reproduce the hardware on your own, you can 3D-print this part with ABS material and install M2 nuts at the positions marked by red arrows. |
| Motor4 Back Cable | <img src="./Metal_Parts/images/02_Motor_Back_Spacer.png" width="80"> | 2-Motor_Back_Spacer.step | Aluminum Alloy 5052 | 1 | CNC |  |
| Link4-5_L | <img src="./Metal_Parts/images/Link4-5_L.png" width="80"> | 2-LINK-4_5-L.step | Aluminum Alloy 5052 | 1 | CNC | |
| Link4-5_R | <img src="./Metal_Parts/images/Link4-5_R.png" width="80"> | 2-LINK-4_5-R.step | Aluminum Alloy 5052 | 1 | CNC | |
| Link5 | <img src="./Metal_Parts/images/Link5.png" width="80"> | 2-RSM5-STATOR.step | Aluminum Alloy 5052 | 1 | CNC | |
|Wrist_Connector_A | <img src="./Metal_Parts/images/Wrist_Connector_A.png" width="80"> | 2-RSM6-RORATOR-1.step | Aluminum Alloy 5052 | 1 | CNC |  |
|Wrist_Connector_B | <img src="./Metal_Parts/images/Wrist_Connector_B.png" width="80"> | 2-RSM6-RORATOR-2.step | Aluminum Alloy 5052 | 1 | CNC |  |
| Gripper Connector A | <img src="./Metal_Parts/images/02_Gripper_Connector_A.png" width="80"> | 2-M6-ROTOR.step  | Aluminum Alloy 5052 | 1 | CNC | |
| Gripper Connector B | <img src="./Metal_Parts/images/02_Gripper_Connector_B.png" width="80"> | 2-M7-STATOR.step  | Aluminum Alloy 5052 | 1 | CNC | |
| Gripper Slider Metal Bracket | <img src="./Metal_Parts/images/02_Slider_Bracket.png" width="80"> | 2-RAIL-BASE-1.step | Aluminum Alloy 5052 | 1 | CNC | Can be 3D printed in ABS with high infill, not recommended for long-term use |
| Slider to Gripper Extension | <img src="./Metal_Parts/images/02_Slider_Extension.png" width="80"> | 2-SLIDER-FIX.step | Aluminum Alloy 5052 | 2 | CNC | |
| Rack | <img src="./Metal_Parts/images/Rack.png" width="80"> | 2-RACK-1M.step | Aluminum Alloy 5052 | 2 | CNC | |


### 🧩 Machining Specifications
- Key dimension tolerance: ±0.02 mm GB/T1840-M
- Surface finish: Anodizing / Sandblasting
- Mating parts recommended: H7 / interference fit
---

## 🛒 Purchased Parts (Standard Parts)

> [!WARNING]
> Since everyone will need to assemble and tighten the screws themselves, standard hex socket screws have been selected. After prolonged operation, the screws may loosen, which will affect the precision of the robotic arm. For this reason, you are required to purchase additional hot melt glue to perform thread locking on the screws at each joint.

If you have a power drill or similar tools, you may choose to buy lock washers or thread-locking screws instead. However, **it is extremely important** that you use the lowest torque setting when using an electric screwdriver to avoid thread stripping, which will result in irreversible damage.


  | Name | Specification / Model | Quantity | Reference Price | Notes |
  |------|----------|------|----------|------|
  | Brushless motor | RobStride RS00 | 4 | 125 $/unit | [SeeedStudio](https://www.seeedstudio.com/Robostride-00-Actuator-p-6664.html) |
  | Brushless motor | RobStride RS06 | 3 | 210 $/unit |  [SeeedStudio](https://www.seeedstudio.com/Robostride-06-Actuator-p-6668.html)  |
  | CAN-USB driver board |  | 1 | 15 $/unit |   [SeeedStudio](https://www.amazon.com/Xiusiyt-Converter-Preloaded-PCAN-Firmware/dp/B0GBW7RTXD/ref=sr_1_2?crid=UNQHGEOCWEW4&dib=eyJ2IjoiMSJ9.BLjBmjTT73o_0hvb0ehHo3M2x1HYsciLqAZy-tlc_uo2eQn5T3jiElnghuDt__xr44HPQx8PITdTIyUG2aWDLwwAktkkejQPPmBc1dzKJXtZrK85hqgBHwCYeY-d8flD_XqsGw94kntXSOp-YSFCBZs-mBO2zVKZuQ6r_JoTjpZHNdDgWz9kMXtI7InFWPrKfV43IkBVJ6gssLjPd9ewBZyYVLORxBKVA6loljry6s1oEOVNtS3ChuU1bMmFcJNrZYlIJp0hqQkzS8kUxo3YIUQsO0GsdaxgyAIP2dpPNdw.O_Y2ZhdC1FWJ-A2gPo5jJHdw92tFf5LuHE9-oElawpA&dib_tag=se&keywords=Pcan&qid=1783575578&sprefix=pcan%2Caps%2C631&sr=8-2)   |
  | XT30 2+2 Power Separation Borrd |  | 1 | 15 $/unit |   [SeeedStudio](https://www.seeedstudio.com/XT30-2-2-Power-Separation-Board-p-6707.html)   |
  | Bearing | 6803ZZ | 3 | 13 $/unit | [Amazong](https://www.amazon.com/uxcell-17x26x5mm-Shielded-Precision-Lubricated/dp/B0D54JSWBZ/ref=sr_1_1?crid=17L94NDI1JCC0&dib=eyJ2IjoiMSJ9.xH_s9Ui7VlS40EZvr-HektqY3VOJsM-VjyE6JaJEScIWuFZ2UYSM7G8j1fC0HSmbb7YlA0YfUxxCkUzBptwrEEdEHsP94TGplNpPAWwhnH8b76HapXR_uHbr1vu3xe0AYSYP30Quk9LMQrGjUh84bXL82z2mORuiri0VHqo5DmSguK0cHubmVaXtbR_eJ43Z7L2nNqWfgltqzmHsYm7DQvrnIBg9UMlD1o9559nCSKA.E_N7CDPQhShckT-1vHDhYvNgiqRKusa12d43hqATQ5A&dib_tag=se&keywords=6803ZZ&qid=1774771801&sprefix=6803zz%2Caps%2C397&sr=8-1) |
  | Bearing | AXK5578 | 1 | 12 $/unit | [Amazong](https://www.amazon.com/PZRT-AXK5578-Thrust-Bearings-Washers/dp/B0B3M3RZGW/ref=sr_1_1?dib=eyJ2IjoiMSJ9.TatYkzOvpYAJ5K23C7Qr9JKJsPhpJE8p1L3k5_1YqQ7ozSLNgOBEeG9pTYz-WXOWiHkbJq_zZR4FxNHAJZ4euyfOGXkOKycOyN0pUD0_WkJia0PekbRy0sYvyQbE7KZByR-40WiPSPuUcysFewSngPoDGQZzESFOUz__V9ViGCIQAPfdUe2OxVpvtbKZYCQsrSDm8b8okR25bavCvpDbBfPh0He2PEBEpl55L8RtYKmlv62XJyfYT1o29A7wO5n8-g3hpJOrKmmWCybdEEWSmquAT1cjvsPTJDaT_TICsso.6xR5pEGJgTR-u_NOyXxi8VTphoLytGd8zugy1-xu-fE&dib_tag=se&keywords=AXK5578&qid=1774771826&sr=8-1&th=1) |
  | Linear rail | MGN9-170mm | 1 | 23 $/unit | [Amazong](https://www.amazon.com/uxcell-Sliding-Carriage-Bearing-Printers/dp/B0D54L45WM/ref=sr_1_1?dib=eyJ2IjoiMSJ9.qNphfY5r4UgLDHslIliMBhC45qBKTl37lJseObJSBp79RJ4VJnAH-lYAMo-rwPiu_uqWmkN7ms4kfAokYvod1seWb5-z2_kVgVuzrCXdiRycNXjrdv3qi5Awuno0_vEqjT4WJ569tAmqm_Rujrdxss7VfpLizFxq6-R8DucuvqZ0M0Y4go9PzRFEFPu4csskz7-UkM1CUidHoKmrT-I7R1Ta0dijj2SYlR_zW0si75k.nRJTebbqw-bFyzkdU8MztHnGdt9qwnHr_gIqa-MDxEQ&dib_tag=se&keywords=MGN9&qid=1774771864&sr=8-1) |
  | Slider block | MGN9 | 2 | 10 $/unit | [Amazong](https://www.amazon.com/uxcell-Bearing-Sliding-Carriage-Anti-Fall/dp/B0D9QBQDKB/ref=sr_1_8?dib=eyJ2IjoiMSJ9.qNphfY5r4UgLDHslIliMBhC45qBKTl37lJseObJSBp79RJ4VJnAH-lYAMo-rwPiu_uqWmkN7ms4kfAokYvod1seWb5-z2_kVgVuzrCXdiRycNXjrdv3qi5Awuno0_vEqjT4WJ569tAmqm_Rujrdxss7VfpLizFxq6-R8DucuvqZ0M0Y4go9PzRFEFPu4csskz7-UkM1CUidHoKmrT-I7R1Ta0dijj2SYlR_zW0si75k.nRJTebbqw-bFyzkdU8MztHnGdt9qwnHr_gIqa-MDxEQ&dib_tag=se&keywords=MGN9&qid=1774771864&sr=8-8) |
  | Gear | Module 1, boss type, 16 teeth, 6 mm bore | 1 | 44$/unit | [Amazong](https://www.amazon.com/Module-15-Teeth-Finished-Perforation/dp/B0GDSR1LKM/ref=sr_1_1?crid=2EN1YHE8TEC58&dib=eyJ2IjoiMSJ9.54N73iSlush8K1a_teRazjBGZaQnbFM4MLysEbIq430CEYcVs0slm8KhpC_JlmjyVMocPA3vLANjERYZWweRag36NhX2GGldVTpd31kAWW4.ws8l0qBABmSVrUGX4g2o3sBbUgOnNhl3Nx_Nt-d1HT8&dib_tag=se&keywords=1%2Bmodule16%2Bteeth&qid=1774772022&sprefix=1%2BModule16%2Bteeth%2Caps%2C403&sr=8-1&th=1)  |
  | Silicone pad | 30x9x2mm | 1 | 10 $ | [Amazong](https://www.amazon.com/Self-Adhesive-Anti-Sliding-Anti-Scratch-Protectors-Appliances/dp/B0F9KVYXFZ/ref=sr_1_3?crid=LVY2LLBFQT6J&dib=eyJ2IjoiMSJ9.4qjOEtjEph1QxS_kJF2vIYqvD_8Lzt4GZ2rrywWbrAhniBvp_8YrEsVNcCPQofO4jVqBxFE8Yplyg2XXgAXlUZwzqE-Gp8MYcaPmphL8Mc1n-ARSCNaTq5gc7ZIWsS6u-kR0G2BzIlBo6NF88KvASjKYJfTHpPXHfNCPVw13P-PseVbUZwlVAO9zMHa3a84gHRd-I-mGB8SCmek9mXjN-c-bFxKvJXlz4C5YBBdt9cH3QkSmLgiLZ_iD4K1mh-MwI5WuVOXr5ZOwJ0bVpmHpc_vpbKLr7CkVack3nsC-TM0.40ujhwS5ConOfA8io_c5hcdos70HOKjMFqqKLKgNwI8&dib_tag=se&keywords=silicone%2Bsticker&qid=1774772199&sprefix=silicone%2Bsticker%2Caps%2C380&sr=8-3&th=1) |
  | Screw | KM3*7mm screw | 80+ |  |[Amazong](https://www.amazon.com/Uxcell-a16011300ux0872-M3x12mm-Carbon-Countersunk/dp/B01E6EIC2S/ref=sr_1_1?crid=2VJKS347LBDWD&dib=eyJ2IjoiMSJ9.eXF2FHahloRY0Kq8sM_EkJUm7ipUgMoVSuTAPjt3ZnAINqLrPQz9A55XDHfe00KPGG3Sr1IJJQloiw7IFwewoPsbdnKBZH5JjT4Ijy_bUXju1IvrHWP4nWeYW1o29jlbHBKEa3fPl8-JzEHr9RPKe5h_Dr1vN6VFMUfszTDEzufQrIi22AsKCMTep5n0-IR7AIc7Fai93nmr4ax8USKGOD_3yu4ri0p8ClPTZzfwmDJvnTpE9J9PNN8uA-wDz72RADQu2VLry_mvb5CA1JV0vHP49Qsy-96MKXo-j3vT8m0.DWiT1Loy7A-MeTveRzxU47S6WCKwnW6MVnmpF256j-s&dib_tag=se&keywords=screw+KM3*12&qid=1776330785&s=industrial&sprefix=screw+km3+%2Cindustrial%2C984&sr=1-1)   |
  | Screw | KM3*16mm screw | 8+ |  |[Amazong](https://www.amazon.com/Uxcell-a16011300ux0872-M3x12mm-Carbon-Countersunk/dp/B01E6EIC2S/ref=sr_1_1?crid=2VJKS347LBDWD&dib=eyJ2IjoiMSJ9.eXF2FHahloRY0Kq8sM_EkJUm7ipUgMoVSuTAPjt3ZnAINqLrPQz9A55XDHfe00KPGG3Sr1IJJQloiw7IFwewoPsbdnKBZH5JjT4Ijy_bUXju1IvrHWP4nWeYW1o29jlbHBKEa3fPl8-JzEHr9RPKe5h_Dr1vN6VFMUfszTDEzufQrIi22AsKCMTep5n0-IR7AIc7Fai93nmr4ax8USKGOD_3yu4ri0p8ClPTZzfwmDJvnTpE9J9PNN8uA-wDz72RADQu2VLry_mvb5CA1JV0vHP49Qsy-96MKXo-j3vT8m0.DWiT1Loy7A-MeTveRzxU47S6WCKwnW6MVnmpF256j-s&dib_tag=se&keywords=screw+KM3*12&qid=1776330785&s=industrial&sprefix=screw+km3+%2Cindustrial%2C984&sr=1-1)   |
  | Screw | KA3*12mm | 48+ |  | [Amazong](https://www.amazon.com/uxcell-Phillips-Tapping-Screws-Silver/dp/B01MXSS95N/ref=sr_1_3?crid=2RJ5ZBG0M4EX5&dib=eyJ2IjoiMSJ9.v9AtN0DrK0YdOT84Puh29n1VDClJz4OwvslbH610w0_xJIkuVFk81UxgSw_lSRbHugpqkja4rz-elY-DHbh0KN4GCFH2MlZhRFjXVE1vlaChALTqgr9jxatNPvPTf8SzdxFoEMEPm3jwCnC8vqLq5xL-Wr414hMsTbVYxv_ZVmEbMV-8YYXhLWiOz9EivU2C8jWw0RFSwVtUxqhj7qgBBYV5QbJRNr1XdWmQsICMHTHy35DeIcLjyKtXOb0gEwDNyqqmdvS5LfJJaLQchjLpW1jondo5xapQVw8gWJ4yYjk.oXwiRL9W52Tlu7tMi7tT9i7g-CBYfw_AAT1LURe2Q7k&dib_tag=se&keywords=screw+ka3*12&qid=1776331569&s=industrial&sprefix=screw+ka3+%2Cindustrial%2C466&sr=1-3)  |
  | Screw | HM3-8mm screw | 60+ |  | [Amazong](https://www.amazon.com/BNUOK-120pcs-Stainless-Threads-Spanner/dp/B0DJQG5YLF/ref=sr_1_4?crid=3J1D711FNBYR9&dib=eyJ2IjoiMSJ9.wo20uXEJsuYS5OBVpnH9TILDd6HtQrJUlEvvYFPE5VV6bozIiRlWwmDaoYnp345KjXwRyxbEgEaRD8gVD2vVhPXg3M266n3H8t9cWN518aR4c5WkFUkqLIqLwdGYBllKcQQ8agsrZYgSVFp9G8LJR4l9oAj8Yx4QN8MReo2k23RVk-lkWeJk1azXD88GFTmd17aiXz6fwOE45Krj4VRiy1oskx8QvMprmJXtH8KowAJo-pWdBtePCCIUUa8oLR78hi17yW_OGJattIwdAziX9RizLI-EMh3hku42WJWnb3g.lZYqsYfJunSoEUPNT04E1sFhPiudREmrI0919PaPBYI&dib_tag=se&keywords=screw%2BHM3-12mm&qid=1776330531&s=industrial&sprefix=screw%2Bhm3-12mm%2Cindustrial%2C475&sr=1-4&th=1)  |
  | Screw | HM3-30mm screw | 16+ |  | [Amazong](https://www.amazon.com/BNUOK-120pcs-Stainless-Threads-Spanner/dp/B0DJQFGRPQ/ref=sr_1_4?crid=3J1D711FNBYR9&dib=eyJ2IjoiMSJ9.wo20uXEJsuYS5OBVpnH9TILDd6HtQrJUlEvvYFPE5VV6bozIiRlWwmDaoYnp345KjXwRyxbEgEaRD8gVD2vVhPXg3M266n3H8t9cWN518aR4c5WkFUkqLIqLwdGYBllKcQQ8agsrZYgSVFp9G8LJR4l9oAj8Yx4QN8MReo2k23RVk-lkWeJk1azXD88GFTmd17aiXz6fwOE45Krj4VRiy1oskx8QvMprmJXtH8KowAJo-pWdBtePCCIUUa8oLR78hi17yW_OGJattIwdAziX9RizLI-EMh3hku42WJWnb3g.lZYqsYfJunSoEUPNT04E1sFhPiudREmrI0919PaPBYI&dib_tag=se&keywords=screw%2BHM3-12mm&qid=1776330531&s=industrial&sprefix=screw%2Bhm3-12mm%2Cindustrial%2C475&sr=1-4&th=1) 
  | Screw | HM4-8mm set screw | 6+ |  | [Amazong](https://www.amazon.com/iexcell-Partially-Threaded-Thread-Socket/dp/B0DR1NX178/ref=sr_1_1?crid=35DT1MLQCOR9C&dib=eyJ2IjoiMSJ9.RlFuoSyG6Yoi2cmVkd0sQ47UpPY4y8uvofyrje4Ha76Dj6dcpknwvFT7DGc5jFqxw5Zd5g4SV-yre7xcMb3WB7MbBowQO3ZzvCgpYWcJ2xzphgz9gx0SNIr_ggqvFcAmxkNuMMVf0p9vPY-jJ2j9cbIk8IwMHlTo6kkuBINPotouNNyElpiy9qHhllwajmKY5v5uDIzJKNJvmhpUtJsd5IS7TB9VaRPkzsDbMDfR4pvs4JgNbU1Zmcu4Ex9fYcRHrOGjAZbbvNxo1r_N5MBKWbxbtZEDDKP_8Oyhgakhhnc.MTLa-_9PBksy6Qge1YqQmlejVfLKkuxB9gT-ZnB9ek0&dib_tag=se&keywords=screw+HM4-75&qid=1776330730&s=industrial&sprefix=screw+m4-75%2Cindustrial%2C401&sr=1-1)  |
  | Screw | HM4-16mm set screw | 18+ |  | [Amazong](https://www.amazon.com/iexcell-Partially-Threaded-Thread-Socket/dp/B0DR1NX178/ref=sr_1_1?crid=35DT1MLQCOR9C&dib=eyJ2IjoiMSJ9.RlFuoSyG6Yoi2cmVkd0sQ47UpPY4y8uvofyrje4Ha76Dj6dcpknwvFT7DGc5jFqxw5Zd5g4SV-yre7xcMb3WB7MbBowQO3ZzvCgpYWcJ2xzphgz9gx0SNIr_ggqvFcAmxkNuMMVf0p9vPY-jJ2j9cbIk8IwMHlTo6kkuBINPotouNNyElpiy9qHhllwajmKY5v5uDIzJKNJvmhpUtJsd5IS7TB9VaRPkzsDbMDfR4pvs4JgNbU1Zmcu4Ex9fYcRHrOGjAZbbvNxo1r_N5MBKWbxbtZEDDKP_8Oyhgakhhnc.MTLa-_9PBksy6Qge1YqQmlejVfLKkuxB9gT-ZnB9ek0&dib_tag=se&keywords=screw+HM4-75&qid=1776330730&s=industrial&sprefix=screw+m4-75%2Cindustrial%2C401&sr=1-1)  |
  | Screw | HM4-70mm set screw | 4+ |  | [Amazong](https://www.amazon.com/iexcell-Partially-Threaded-Thread-Socket/dp/B0DR1NX178/ref=sr_1_1?crid=35DT1MLQCOR9C&dib=eyJ2IjoiMSJ9.RlFuoSyG6Yoi2cmVkd0sQ47UpPY4y8uvofyrje4Ha76Dj6dcpknwvFT7DGc5jFqxw5Zd5g4SV-yre7xcMb3WB7MbBowQO3ZzvCgpYWcJ2xzphgz9gx0SNIr_ggqvFcAmxkNuMMVf0p9vPY-jJ2j9cbIk8IwMHlTo6kkuBINPotouNNyElpiy9qHhllwajmKY5v5uDIzJKNJvmhpUtJsd5IS7TB9VaRPkzsDbMDfR4pvs4JgNbU1Zmcu4Ex9fYcRHrOGjAZbbvNxo1r_N5MBKWbxbtZEDDKP_8Oyhgakhhnc.MTLa-_9PBksy6Qge1YqQmlejVfLKkuxB9gT-ZnB9ek0&dib_tag=se&keywords=screw+HM4-75&qid=1776330730&s=industrial&sprefix=screw+m4-75%2Cindustrial%2C401&sr=1-1)  |
 | Screw | HM3-6mm screw | 8+ |  | [Amazong](https://www.amazon.com/BNUOK-120pcs-Stainless-Threads-Spanner/dp/B0DJQG5YLF/ref=sr_1_4?crid=3J1D711FNBYR9&dib=eyJ2IjoiMSJ9.wo20uXEJsuYS5OBVpnH9TILDd6HtQrJUlEvvYFPE5VV6bozIiRlWwmDaoYnp345KjXwRyxbEgEaRD8gVD2vVhPXg3M266n3H8t9cWN518aR4c5WkFUkqLIqLwdGYBllKcQQ8agsrZYgSVFp9G8LJR4l9oAj8Yx4QN8MReo2k23RVk-lkWeJk1azXD88GFTmd17aiXz6fwOE45Krj4VRiy1oskx8QvMprmJXtH8KowAJo-pWdBtePCCIUUa8oLR78hi17yW_OGJattIwdAziX9RizLI-EMh3hku42WJWnb3g.lZYqsYfJunSoEUPNT04E1sFhPiudREmrI0919PaPBYI&dib_tag=se&keywords=screw%2BHM3-12mm&qid=1776330531&s=industrial&sprefix=screw%2Bhm3-12mm%2Cindustrial%2C475&sr=1-4&th=1)  |
 | Screw | HM3-26mm screw | 6+ |  | [Amazong](https://www.amazon.com/BNUOK-120pcs-Stainless-Threads-Spanner/dp/B0DJQG5YLF/ref=sr_1_4?crid=3J1D711FNBYR9&dib=eyJ2IjoiMSJ9.wo20uXEJsuYS5OBVpnH9TILDd6HtQrJUlEvvYFPE5VV6bozIiRlWwmDaoYnp345KjXwRyxbEgEaRD8gVD2vVhPXg3M266n3H8t9cWN518aR4c5WkFUkqLIqLwdGYBllKcQQ8agsrZYgSVFp9G8LJR4l9oAj8Yx4QN8MReo2k23RVk-lkWeJk1azXD88GFTmd17aiXz6fwOE45Krj4VRiy1oskx8QvMprmJXtH8KowAJo-pWdBtePCCIUUa8oLR78hi17yW_OGJattIwdAziX9RizLI-EMh3hku42WJWnb3g.lZYqsYfJunSoEUPNT04E1sFhPiudREmrI0919PaPBYI&dib_tag=se&keywords=screw%2BHM3-12mm&qid=1776330531&s=industrial&sprefix=screw%2Bhm3-12mm%2Cindustrial%2C475&sr=1-4&th=1)  |
 | XT30 2+2 Cable | Two Side Elbows 320mm | 1+ |  <img src="./Metal_Parts/images/XT30.png" width="80"> | This will require custom fabrication on your end.  |
 | XT30 2+2 Cable | Two Side Elbows 200mm | 4+ |  <img src="./Metal_Parts/images/XT30.png" width="80"> | This will require custom fabrication on your end.  |
 | XT30 2+2 Cable | One Side Elbow 300mm| 1+ |  <img src="./Metal_Parts/images/XT30.png" width="80"> |  This will require custom fabrication on your end. |
 | XT30 2+2 Cable | Two Side Straight | 1+ |  |   |
  | Screwdriver set | Hex key set | 1 | 16$  | [Amazong](https://www.amazon.com/Amazon-Basics-Ratcheting-Electronics-Screwdriver/dp/B07V4TFWFZ/ref=sr_1_2?crid=ADAY70RZDSLN&dib=eyJ2IjoiMSJ9.jcLL4o6IXTnPlPfTTzbCZCBuZx2sLkvdUQCwlL58aq__GOyLxVPnwLI0mvGptba_HeVz6ctLQ_ziQw56BMDH9IOaw-4PVJGMktQM74mWficwggm3ckDGyAH-agN_zkB3K0_W-wrS56jfcMYFbZSWhWxr-iSOC4sdXwMGlt4rYGtenyn9yAFYBIHqjU2El5_OAKuspsrF0yQvfyfQPQHs46SClWN8zlSemGVZRuVSU26f0f9yApF6BfWHANKNNhT0Mfb6bQ8oM2XUMvwaazrrKoHeTARuoflVaVZvMU776bs.r8gy_gMINEy0qy4JyK--z-IbPZEv-SWeMGohOOE7M60&dib_tag=se&keywords=Screwdriver+set&qid=1774772499&s=industrial&sprefix=screwdriver+set+%2Cindustrial%2C374&sr=1-2)  |



### About Fixing
You may modify your base freely based on the 3D printed parts we provide. You can also use G-clamps according to the thickness of your desktop.

  | Name | Specification / Model | Quantity | Reference Price | Notes |
  |------|----------|------|----------|------|
  | Woodworking clamp | 6-inch G clamp | 2 | 20 $/unit | [Amazong](https://www.amazon.com/gp/aw/d/B092J1YW2M/?_encoding=UTF8&pd_rd_plhdr=t&aaxitk=3557c048ce58e7dbb50b40c3af69f1d6&hsa_cr_id=0&qid=1774772748&sr=1-1-9e67e56a-6f64-441f-a281-df67fc737124&ref_=sbx_s_sparkle_sbtcd_asin_0_img&pd_rd_w=bNqtC&content-id=amzn1.sym.2fb72bc8-96ef-420d-b08f-c04b69f36507%3Aamzn1.sym.2fb72bc8-96ef-420d-b08f-c04b69f36507&pf_rd_p=2fb72bc8-96ef-420d-b08f-c04b69f36507&pf_rd_r=KDCPNZRHFWEWBWVHWSTR&pd_rd_wg=sBvfF&pd_rd_r=52b946ee-46e2-4e74-86ee-99e291552e44) |



### About Power Supply
The robotic arm is shipped without a power supply by default. You may connect your own battery, or purchase a reliable 48V 12.5A MeanWell power supply made in Taiwan. Additionally, you will need to buy a three-pin plug compliant with local standards and a wiring harness with XT30 female connector.

#### Consumables BOM

| Name | Specification | Qty | Reference Price | Notes | Image |
|:---|:---|:---:|:---:|:---|:---:|
| Power Supply | LRS-600-48（48V12.5A） | 1 | $69.5 | [amazon](https://www.amazon.com/LRS-600-48-Switching-Upgrade-Version-SE-600-48/dp/B0BV5XFYNS/ref=sr_1_1?crid=2MK5Y1UI66CW9&dib=eyJ2IjoiMSJ9.FAt8rrpVeLIbeU2px5Bpe3WU2xsHpE3Kw1Fc6ZdPBFrIpRsaASOwU1dL9jPUNnpXO5u67hvlSXTsKCXH7jehZ8VWfiSFbcHmsVhJY_ua86iPUltJFeWlT9LIXphFER27jHWGnaJb2NdRIpPBMVdae8qgIllUI1J-Q8pZranpyjkkiJP2RmiEdhUBXTvvH3-vhk8z2uhf7BJrGW7hjRbjyCO7WHwwBQ3tMcnEKwto2doy9qus35djHRzODSFPbMuiA66PdgPuib4VL1aQghehDEiceMIpTUiCHHeRHfpB71M._yrosm8mVfpUq-5PjNTLSaYPgv8Dot6YbQTaGULjlLQ&dib_tag=se&keywords=LRS-600-48&qid=1781762081&s=electronics&sprefix=lrs-600-48%2Celectronics%2C351&sr=1-1) | <img src="./Purchased_Parts/LRS-600-48.png" width="80"> |
| Power Cord | US Standard AC Cable | 1 | $4.49 | [amazon](https://www.amazon.com/LIFEPOE-Power-3-3ft-Black-3-Prong/dp/B0FK4KPW2G/ref=sr_1_1?crid=2W5766PT8EOKA&dib=eyJ2IjoiMSJ9.7E5s-9-Zh-jJAdni-17Iyt1Mr3GJD6hMt9pfk-0S5YxZtknZik9OiePitwUom0pYUbePRpdqa0dCZtGUjluQDEJbSDePHCGvBV6bwQU7wfwd0Loo4WJJmH_2CM1KRKSPcxHXRH0i1i5yuy4g7fDxxn3nPGYU3aF00m5jiIkMfYFgOxH4yURjjZeTMZAIO9wiVQUsPrlM51UIgpPo2YYdCQVUsxjumSsTAm0Jpt2SsBEdT-QzXSIKpLSvQ6kGijXF-4ZevaxiShJdmwU8t2LobDLcalXEOl3lriZTGhjwxow.r0oBabUkGwewhvO3IKlBMULdhUSe6yNTsjfFUaBsjyU&dib_tag=se&keywords=US%2BStandard%2BAC%2BCable%3B%2B1.5m%2B-%2B3%2B*%2B1.5mm%C2%B2&nsdOptOutParam=true&qid=1780021862&s=industrial&sprefix=lrs-350-24%2Cindustrial%2C387&sr=1-1&th=1) | <img src="./Purchased_Parts/US Standard AC Cable.png" width="80"> |
| Output Port | XT60E Fixed Female Connector; XT60E Female + Lug - 10cm; 4mm Lug Hole | 1 | $9.99 | [amazon](https://www.amazon.com/LINSYRC-XT60E-F-Connector-Battery-Quadcopter/dp/B0CQK1P1DP/ref=pd_sbs_d_sccl_1_2/133-3898271-3474923?pd_rd_w=FmCVA&content-id=amzn1.sym.aa738fbd-ad05-4d11-aae2-04b598db6305&pf_rd_p=aa738fbd-ad05-4d11-aae2-04b598db6305&pf_rd_r=03QM0MRVZA968N9X6X6E&pd_rd_wg=WOZ9q&pd_rd_r=6e0577d2-de73-4427-affd-a271808e1453&pd_rd_i=B0CQK1P1DP&psc=1) | <img src="./Purchased_Parts/XT60E Female to Copper Lug Pigtail.png" width="80"> |
| Power AC Wiring | 1.5mm²; Red, Blue, Yellow x1 each(User must crimp terminals to the wire — pre-crimped leads not included.); 10CM | 3 | $0.99 | [aliexpress](https://www.aliexpress.com/item/1005008648016252.html?spm=a2g0o.productlist.main.2.15c9ZpluZpluHP&algo_pvid=09efee83-d80c-4ece-b588-3b1ef73279a3&algo_exp_id=09efee83-d80c-4ece-b588-3b1ef73279a3-1&pdp_ext_f=%7B%22order%22%3A%22230%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21USD%213.58%210.99%21%21%2124.09%216.65%21%400b0b305117800339070873795e0f3d%2112000046086542230%21sea%21US%216593543849%21ABX%211%210%21n_tag%3A-29910%3Bd%3A518b3f9d%3Bm03_new_user%3A-29895%3BpisId%3A5000000207178484&curPageLogUid=74aJ9L7lm7hs&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008648016252%7C_p_origin_prod%3A&gatewayAdapt=4itemAdapt) | <img src="./Purchased_Parts/RV Grounding Wire Coil with Y-Terminal Lugs.png" width="80"> |
| 3-in-1 IEC Inlet Socket | Quick-connect type with red switch (Dual Nuts) | 1 | $1.98 | [aliexpress](https://www.aliexpress.com/item/1005005962021242.html?spm=a2g0o.imagesearchproductlist.main.17.7db7cZZdcZZdCY&algo_pvid=270b0987-1973-41ad-a2b9-6fe008f9edb5&algo_exp_id=270b0987-1973-41ad-a2b9-6fe008f9edb5&pdp_ext_f=%7B%22order%22%3A%22346%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21USD%213.31%211.98%21%21%2122.30%2113.35%21%400b0b305117800327806706342e118f%2112000035062406338%21sea%21US%216593543849%21ABX%211%210%21n_tag%3A-29910%3Bd%3A518b3f9d%3Bm03_new_user%3A-29895%3BpisId%3A5000000204886261&curPageLogUid=87JUDbPbch2i&utparam-url=scene%3Aimage_search%7Cquery_from%3Apc_web_image_search%7Cx_object_id%3A1005005962021242%7C_p_origin_prod%3A) | <img src="./Purchased_Parts/3-in-1 IEC Inlet Socket.png" width="80"> |
| XT30 to XT60 adapter cable plug | XT30U female to XT60 male | 1 | 8.99$ | [amazon](https://www.amazon.com/dp/B0BY8PSHK6?th=1) | <img src="./Purchased_Parts/XT30U_female_to_XT60_male.png" width="80"> |
| 304 Stainless Steel Phillips Countersunk Head Screw | M4x6 | 10 | $0.37 | / | / |
| 304 Stainless Steel Phillips Countersunk Head Screw | M3x8 | 2 | $0.36 | / | / |
| 304 Stainless Steel Phillips Pan Head Screw | M3x8 | 2 | $0.32 | / | / |
| Hex Nut | M3x2.5 | 2 | 2.10 CNY | / | / |

Printed Parts BOM:

| Name | Image | Quantity | Notes |
| ------ | ---- | --- | ---- |
| [Front Shell](./3D_Printed_Parts/RS-power-Top%20Cover.stp) | <img src="./3D_Printed_Parts/images/RS-power-Top Cover.png" width="80"> | 1 | PLA 0.4 nozzle, 0.2 layer height, 30% infill |
| [Rear Shell](./3D_Printed_Parts/RS-power-Bottom%20Cover.stp) | <img src="./3D_Printed_Parts/images/RS-power-Bottom Cover.png" width="80"> | 1 | PLA 0.4 nozzle, 0.2 layer height, 30% infill |
| [Front Shell (Sliding Cover)](./3D_Printed_Parts/RS-power-Top%20Cover-Sliding%20Cover.stp) | <img src="./3D_Printed_Parts/images/RS-power-Top Cover-Sliding Cover.png" width="80"> | 1 | PLA 0.4 nozzle, 0.2 layer height, 30% infill |

#### Power Supply Assembly

- The power supply assembly steps are divided into two parts: front shell and rear shell:

##### 1. Front Shell Assembly

| Step | Description | Image | Notes |
|:---:|---|---|---|
| 1-1 | Prepare the parts and printed components required for front shell assembly | <img src="./Assembly_Steps/powerstep_images/1-1.png" width="80"> | Check that all parts are present |
| 1-2 | Wiring sequence instructions for each part; assemble according to the wiring sequence | <img src="./Assembly_Steps/powerstep_images/1-2(1).png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-2(2).png" width="80"><br><img src="./Assembly_Steps/powerstep_images/1-2(3).png" width="80"> | Connect strictly according to the wiring sequence |
| 1-3 | Install the XT60 connector | <img src="./Assembly_Steps/powerstep_images/1-3（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-3（2）.png" width="80"> | Secure with M3x8 304 countersunk cross-head screws and M3x2.5 hex nuts |
| 1-4 | Install the 3-in-1 IEC socket | <img src="./Assembly_Steps/powerstep_images/1-4（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-4（2）.png" width="80"> | Secure the 3-in-1 IEC socket with M3x8 304 pan head cross-head screws |
| 1-5 | Internal wiring of the front shell | <img src="./Assembly_Steps/powerstep_images/1-5（1）.png" width="80"><br><img src="./Assembly_Steps/powerstep_images/1-5（2）.png" width="80"> | Check connections against the wiring diagram |
| 1-6 | Secure the front shell to both sides of the power supply | <img src="./Assembly_Steps/powerstep_images/1-6（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-6（2）.png" width="80"> | 4x M4x6 304 countersunk cross-head screws |
| 1-7 | Install the sliding cover | <img src="./Assembly_Steps/powerstep_images/1-7（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-7(2).png" width="80"> | Push in from the bottom of the power supply |
| 1-8 | Secure the sliding cover | <img src="./Assembly_Steps/powerstep_images/1-8.png" width="80"> | 2x M4x6 304 countersunk cross-head screws |

---

##### 2. Rear Shell Assembly

| Step | Description | Image | Notes |
|:---:|---|---|---|
| 2-1 | Prepare the parts and printed components required for rear shell assembly | <img src="./Assembly_Steps/powerstep_images/2-1.png" width="80"> | Check that all accessories are complete |
| 2-2 | Assemble the rear shell with the power supply | <img src="./Assembly_Steps/powerstep_images/2-2.png" width="80"> | Align the position |
| 2-3 | Secure the rear shell to both sides of the power supply | <img src="./Assembly_Steps/powerstep_images/2-3(1).png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/2-3(2).png" width="80"> | 4x M4x6 304 countersunk cross-head screws |

---

##### 3. Final Completion

| Step | Description | Image | Notes |
|:---:|---|---|---|
| 1 | Power supply assembly completed | <img src="./Assembly_Steps/powerstep_images/3.png" width="80"> | Check that all screws are tightened |

---