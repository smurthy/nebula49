# nebula49
I built a workstation with the System76's Nebula49 case. Based in Denver, System76 is a great local company to work with and have been responsive to my queries. They also own the vertical to their own custom linux distro (PopOS) which I use as a daily driver. 

| Part        | Description |
| ----------- | ----------- |
| CPU         | AMD Threadripper 7960x 24-Core, 48-Thread Processor |
| CPU Cooler  | ARCTIC Freezer 4U-M (Rev. 2) |
| Thermal Paste| Kingpin Cooling KPx Thermal Grease 3g|
| Motherboard | GIGABYTE TRX50 Aero D |
| Power Supply| Pure Power 12 M 1000W |
| RAM         | Kingston Fury DDR5 5600MT/s CL28 1.35V EXPO|
| SSD         | Samsung 990 PRO SSD 4TB PCIe 4.0 M.2 2280|
| GPU         | NVIDIA Quadro M4000 8G|

<img src="https://github.com/user-attachments/assets/72cb25e3-3684-4f42-b0b3-fe692e4cdff7" width="800" height="800">

## The Behemoth
The CPU cooler is clearly the largest piece of equipment in the case. So much so that the CPU duct's own fan bracket does not fit within the dimensions of the Arctic Freezer cooler. 
It has to be removed but the cooler has an exhaust fan and inflow fan attached to the fins to compensate. 

In addition, there's another exhaust fan at the end of the duct that's provided with the case. 
Disabling that exhaust fan does have a negative impact on CPU temps by ~4C on idle. There'll be a larger delta on heavier load. The 3 CPU duct fans, combined, account
for the most noise in the case. Setting these three fans to the *silent profile* either in the motherboard BIOS or through Gigabyte's control software should alleviate some noise concerns -- but recommend to return
to the *normal fan profile* under heavy load.
 
<img src="https://github.com/user-attachments/assets/4a0513c9-2914-4917-bd60-ecd434e6ec20" width="600" height="600">

<img src="https://github.com/user-attachments/assets/4f0d05b1-3680-4836-8922-538d6d020c2f" width="600" height="600">

*CPU cooler with both inlet and exhaust fans attached to the fins*

<img src="https://github.com/user-attachments/assets/b5f4ad41-8c16-4226-803c-dd711a479cda" width="600" height="600">

*Fan bracket inside CPU duct won't fit with the massive Arctic Freezer cooler*


## The Case
The case is the anti-gaming system setup. It's powder coated with 1.6MM 5052 H32 Aluminum. Dark themed and internals closed to the outside world with the exception of holes for air inflow/outflow. 
Even those holes are covered with filters so you can't get a good luck inside. Just as well, nebula49 is designed for optimal thermal and sound performance and it delivers. 

The separated CPU duct creates directional windflow to cool the CPU while the plethora of other fans located above the GPU-area and at the bottom of the case take care of cooling the other components. All of the SSD slots 
have their own heatsinks cooled by the side and bottom fans. 

The 1000W powersupply has it's own directed windflow from the bottom and exits to the back. The fans are engineered to reduce vibrations.

<img src="https://github.com/user-attachments/assets/e3990428-0300-4e59-ba80-37cae941691c" width="600" height="600">

<img src="https://github.com/user-attachments/assets/fdb53504-9169-49d7-88d5-98e1e3b3f8aa" width="600" height="600">

<img src="https://github.com/user-attachments/assets/f7ff283b-3c5a-4e18-b5ad-dc67b827303e" width="600" height="600">

<img src="https://github.com/user-attachments/assets/638fd3e1-8146-46ff-b34b-6e10f93c8468" width="600" height="600">

<img src="https://github.com/user-attachments/assets/af687941-9478-49b9-a2df-da872596649f" width="600" height="600">

<img src="https://github.com/user-attachments/assets/ec21dcbd-30cb-4b67-9d56-2bf7f5dcde0e" width="600" height="600">


<img src="https://github.com/user-attachments/assets/d8ac7fd7-0f07-48bd-882f-da70663fb9fc" width="450" height="450">

*Idle thermals look good*

## Design choices and considerations
While the motherboard does support multiple PCIe Gen5 SSD slots, I opted for a Gen4 SSD at higher capacities and lower price. Reviews indicate the temperature management (even on idle) is still an issue for Gen5 SSDs.
Also, with random I/O, the performance delta is negligble between Gen5 and Gen4. Still, something I might change once the thermal performance (and power draw) improve in future generations of Gen5 SSDs.

The cable management was a painpoint (specifically the power to the motherboard being right underneath the CPU duct). Looking at System76's manual helped me find the optimal routing for wiring. The other painpoint was the flexing of the
PCIe brackets. You can see in above images some are bent inwards and others outwards. I used the Dell T5610 as a comparision of bracket rigidity. It makes life a bit easier when handling and also don't want that metal bracket to touch the motherboard.

The GPU is underwhelming but that's what I had lying around. Since the newer generation entry-level Nvidia PRO cards don't allow sharing memory, I'll need to consider which route to take since VRAM will be important for some of my use cases (not gaming).

By default, the RAM speed is around 4800 MT/s. EXPO must be enabled in the BIOS to reach closer to 5600 MT/s. I opted not to do that for now as the RAM is also a source of heat, power draw. As the Threadripper CPU can easily torch 350 Watts under full load, I'm still tweaking to find the right balance of power and efficiency.
