---
title: "haptic"
author: "JavaScythe"
description: "8 channel 2A motor with flyback protection USB controller with 5 extra exposed GPIOs"
created_at: "2025-6-18"
---

20 Hours total

### 06-18-25: Research and Initation
A post in the r/simracing discord led me to this link: https://www.printables.com/model/1276952-diy-simagic-p-hpr-neo-clone

The motors only 1.5$? Easy steal for something like this. Obviously I wouldn't use the commerical controller they are supposed to work with, so designing my own was the next move.

I decided on 8 channels because while overkill, it keeps the PCB small but still maximizes performance for cost.
<img width="349" alt="image" src="https://github.com/user-attachments/assets/3204866a-318d-4701-89e7-15fbe8974441" />
<img width="281" alt="image" src="https://github.com/user-attachments/assets/c48c7d8b-597a-4d10-8535-4d04d02af6da" />

I looked into some MCUs and FETs on JLCPCB and came up with ATSAMD11D14A and AO3400A, economical and perfect for this use case

1 Hour

### 06-19-25: Schematic Creation
Now to pick parts: USB header, screw terminals, USB protector.

Downloaded the docs for all of them and spent a flight connecting them in schematic, as well as the other components
<img width="898" alt="image" src="https://github.com/user-attachments/assets/caa69491-a48b-4d64-a368-5ec865dd7eb9" />

8 Hours

### 06-21-25: PCB Creation
Routing everything on one layer to preserve the high current ground plane. Each motor is like 2A max max max so this enourmous plane is just fine for 8.

<img width="618" alt="image" src="https://github.com/user-attachments/assets/8e5d8370-56c0-4408-be4f-b173be2a8c54" />

This took another flight and some addtional pre and post time.

7 Hours

### 06-22-25: Part Selection
Finding appropriate JLCPCB parts for PCBA, and uploading the Gerbers to test the prices.

I didn't account for the extended component library or whatever when choosing parts, and those are a 3$ each cost, so I need to find alternatives for those. It was about 56$ with those, and about half of that price was because of the extended.

With replacements for those, the PCB should be about 25$ and that means about 7-8 motors.

<img width="630" alt="image" src="https://github.com/user-attachments/assets/3ba6b8e4-6a66-4576-ad3e-38b53dd84e35" />

2 Hours

### 06-23-25: Swapping extended parts for basic
Changing the pieces did indeed have a great effect on the price
<img width="604" alt="image" src="https://github.com/user-attachments/assets/d5d071d2-ced8-441f-81c6-c3bc40c8564c" />

This means 8x motor will fit confortably in the BOM.

2 Hours
