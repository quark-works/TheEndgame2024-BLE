# This is amodified version of THE ENDGAME keyboard to make it wireless
 This works by using a SuperMini NRF52840 or a nice!nano. Sadly, there's not solution with castellated holes so the soldering is a little bit... special. Here are some pictures of the board:

<img src="https://github.com/quark-works/TheEndgame2024-BLE/blob/main/004%20IMAGES/FRONT-BLE.png" alt="FRONT">

<img src="https://github.com/quark-works/TheEndgame2024-BLE/blob/main/004%20IMAGES/BACK-BLE.png" alt="BACK">


## CASE

There's an updated version of the case with a slot for a battery, please measure which battery will fit as it is a pretty small opening. ZMK is pretty power efficient os that's not an issue.

## FIRMWARE

Included is a precompiled firmware ZMK Studio ready as well as the source I've used.
Additionally there is a VIAL firmware if you are more familiar with that and do not need wireless capability. However you can only use this if you have a pro-micro rp2040 mcu installed on your pcb. Be aware that pinout is not the same as with SuperMini NRF52840 or nice!nano.


## MY BUILD

<img src="https://github.com/quark-works/TheEndgame2024-BLE/blob/main/004%20IMAGES/BLE-BUILD.jpeg" alt="BUILD">

## Caveats:
- Soldering is a little on the harder side. You gotta align the board and feed enough solder so it melts and attaches both the pads on the PCB and the pads on the micro.
- I don't fully like how close the battery pads are. Be careful when you solder the batter. My recommendarion is: Solder one pad, add tape, then solder the other pad.
- I'd love to remake this board to have everything preassembled but this version works well enough. If there's enough interest I might just do it.


## Following is the original GitHub repo content

<img src="https://github.com/OldMan6955/TheEndgame2024/blob/main/004%20IMAGES/TheEndgameBillboard.jpg" alt="TheEndgameBillboard">




## Who the F... is Alice ##


Inspired by the legendary TGR Alice, the ENDGAME pays homage to a true classic. While it might not claim the top spot for ergonomics, it's design speaks for itself an iconic piece you’ll want to show off, even if it takes a bit of time for your fingers to adjust.

This low profile keyboard is built for high performance typing. Its slightly staggered layout works beautifully for both ergonomic beginners and experienced users. The unique bottomless top mount design makes it incredibly slim, lightweight, and perfect for those on the move.



## Everything You Need, All In One Place ##

Get the entire kit from KeebSupply, a trusted vendor with affordable international shipping. It’s your one stop shop for everything you need highly recommended! [Buy here](https://keeb.supply/products/endgame) 

For an excellent build guide, check out this fantastic resource from KeebSupply. I haven’t had the time to create my own guide (and honestly, I couldn’t top this one). Big thanks to @KeebSupply! [Build Guide and Supplies](https://docs.keeb.supply/endgame/) 



## PARTS LIST PCB ##

- 1x The Endgame PCB             [Gerber Files](https://github.com/OldMan6955/TheEndgame2024/tree/main/001%20PCB) 

There are now two versions of the PCB:
1.	COPPER Version:
In this version, all design elements are on the copper and mask layers. I used this version to create my prototypes. However, this version has longer loading times, and the Gerber files currently don’t work with JLCPCB. (I’d greatly appreciate any help with troubleshooting this issue.)
2.	SILKSCREEN Version:
This version is untested. All design elements have been moved to the silkscreen layer, making it much more performant on less powerful PCs. The Gerber files display correctly on JLCPCB but have not yet been tested.
Please always test the files yourself to rule out potential errors. Thank you!

- 36x Choc v1 Hotswap Sockets    [buy here](https://www.aliexpress.com/item/1005004916925259.html?) 
- 36x Diodes SOD123 / 1N4148W T4 [buy here](https://de.aliexpress.com/item/1005004309686841.html?) 
- 1x Waveshare RP2040 UGLY AF    [buy here](https://de.aliexpress.com/item/1005006354505058.html?) 

or get the better looking thingy, highly recommended

- | 01 | 0xCB Gemini             [buy here](https://keeb.supply/products/0xcb-gemini) |



## PARTS LIST FDM CASE ##

- 4x M3 6mm countersunk          [buy here](https://de.aliexpress.com/item/4001199728978.html) 
- 4x M3 5mm flathead             [buy here](https://de.aliexpress.com/item/1005005069968742.html) 

You can choose either countersunk or flathead screws both work well. Countersunk screws automatically align the PCB, while flathead screws allow you to manually align and adjust as needed.
The hole for the heat inserts is 4mm deep, and the PCB is 1.6mm thick, so 5mm screws are a perfect fit. Just double-check how the screw length is measured, as this can vary.

- 4x M3 D4.6mm L3mm Heatinsert   [buy here](https://de.aliexpress.com/item/4000232858343.html) 
- 12x M3 D6.6mm grommet black     [buy here](https://de.aliexpress.com/item/4000712868621.html) 

You’ll need 4 grommets if you’re aiming for a bit of flex or bounce, but you can use up to 12 depending on your preference. They work perfectly as feet and provide excellent grip on my desk. Alternatively, bumpons are a great option too.

## SWITCHES AND KEYCAPS ##

Switches

I highly recommend the Choc v1 Silent switches, such as [Nocturnal](https://keeb.supply/products/nocturnal-low-profile-switches) or [Twilights](https://keeb.supply/products/twilight-low-profile-switches). If you prefer heavier springs and a bit of tactile feedback but don’t need silence, [Sunset](https://keeb.supply/products/sunset-low-profile-switches) switches are an excellent choice. As for the rest of the Choc v1 lineup, I wouldn’t bother—they’re not worth considering.

Keycaps

My go-to choice is standard [MBK](https://keeb.supply/products/mbk-keycaps) keycaps, but personal preference always plays a role. For your setup, you’ll need:

- 30x 1U keycaps for the alpha keys (or 28x 1U and 2x 1U homing keycaps)
- 4x 1.5U and 2x 1U convex keycaps for the bottom row

Check with your local vendor, they’re in stock almost everywhere these days. A great way to test switches and keycaps is by attending meetups, there might be an active community near you.


## FIRMWARE - QMK AND VIAL ##

The firmware, expertly created by [dreipunkteinsvier](https://github.com/dreipunkteinsvier), is available for download: [Get it here](https://github.com/OldMan6955/TheEndgame2024/tree/main/003%20FIRMWARE) 
Huge thanks to him, I’d have been completely lost without his help!

## DISCLAIMER ##

This keyboard is an open-source project, and all files are provided free of charge for personal use. While these files have been tested and worked for me, they are provided without any guarantees or warranties of any kind.

By using these files, you agree to take full responsibility for verifying their suitability for your needs. Any orders, modifications, or reproductions made based on these files are done at your own risk. I am not liable for any issues, damages, or losses that may arise from the use of these files or the assembly of the keyboard.

Please ensure you carefully review all files and specifications before proceeding. Thank you for understanding!

## RANDOM PEOPLE I KNOW ##

After three years of development and collaboration with contributors from around the world, the ENDGAME is more than just a keyboard it’s the result of a shared journey, a community driven effort that reflects the passion and creativity of everyone involved.

- [Marco "Bob"](https://github.com/GroooveBob) - for answering all my dumb questions 24/7
- [dreipunkteinsvier](https://github.com/dreipunkteinsvier) - firmware and stupid github
- [bubbleology](https://github.com/bubbleology) - inspiration, CAD and emotional support
- [GEIST](https://github.com/GEIGEIGEIST) - can't remember what, but we talked about stuff back in the days RIP
- MY WIFE - for reasons
- and many more

To all who contributed thank you. Enjoy the journey, and have fun exploring what this keyboard can do!

## PICTURES ##

<img src="https://github.com/OldMan6955/TheEndgame2024/blob/main/004%20IMAGES/TheEndgameMood.jpg" alt="TheEndgameMood">
<img src="https://github.com/OldMan6955/TheEndgame2024/blob/main/004%20IMAGES/TheENDGAME%20front.png" alt="TheENDGAME front">
<img src="https://github.com/OldMan6955/TheEndgame2024/blob/main/004%20IMAGES/TheENDGAME%20back.png" alt="TheENDGAME back">


## ONLY FANS ##

While this project is free and open source, I truly appreciate your support. If you'd like to contribute, feel free to leave a tip via Ko-fi to help support future projects. Thank you!

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T218HXN9) 

## SHARE YOUR BUILDS ##

Do you love your ENDGAME? I’d love to see your builds! Join the Discord community to share pictures of your keyboards and chat with fellow enthusiasts.
Just a heads-up: I can’t help with technical issues or soldering nightmares because I’m still learning myself. So, please don’t ask me for help with that!

[![Join My Discord](https://img.shields.io/badge/Join%20Me-On%20Discord-7289da?logo=discord&style=for-the-badge)](https://discord.gg/NQmW8mduXG)

## FINAL WISDOM ##

    "The worst thing that can happen is someone calling me a keyboard designer."
    -OLDMAN6955

