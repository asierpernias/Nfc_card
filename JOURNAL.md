### October 2 - 1.1 hours
One of the things I knew I wanted on my business card was an NFC tag, as a way to link my portfolio directly through the card. I started researching which NFC tags I could use. From previous research I knew about the NTAG213, but it was not available in JLCPCB's PCBA option, so I looked for other alternatives. Then I found the ST25TN01K, which met everything I needed. After that I looked up its footprint and symbol and started reading its documentation while experimenting with the design of the copper coil. To get the coil as optimized as possible, I used the NFC Inductance tool from ST, the manufacturer.

[Lapse](https://lapse.hackclub.com/timelapse/ta8I1HCvqRD3)

<img width="1272" height="687" alt="Captura de pantalla 181732" src="https://github.com/user-attachments/assets/78e74143-7faf-43ac-a2e5-cfd76181c5ac" />

### October 2 - 50 min
Once I had a rough idea of the parameters for the copper coil, I started trying to route it. My first idea was to draw it by hand, but even after trying custom rules in KiCad (which I tried to learn along the way) it was too messy. Another option was a KiCad plugin, but I couldn't find one, either in KiCad or on GitHub, that could generate rectangular coils instead of circular ones. Since I was losing my mind, I decided to ask Claude to generate a script, which I then checked and adjusted the parameters of. The script generated a file with a copper coil fully customized for my PCB, since by that point I had already set its dimensions.

<img width="955" height="530" alt="image" src="https://github.com/user-attachments/assets/38282507-fd1f-4844-9179-dd52cfb3fef1" />

### October 2 - 40 min
As shown in the Lapse, once the electrical part was finished I started on the visual design. I designed it in black and white in Figma and then exported it to KiCad. During the process I had a lot of problems converting it to actual silkscreen. I later discovered it was because the images were being exported at a small size. I fixed it by exporting from Figma at 10x and then adjusting the dimensions natively in KiCad.

[Lapse](https://lapse.hackclub.com/timelapse/SvZdMfJdZlAd)

<img width="531" height="336" alt="image" src="https://github.com/user-attachments/assets/e3e3b001-4e41-4536-8cf8-4c8cf5330594" />

### October 3 - 2 hours
This has been much harder than I expected. Today I continued as usual designing more silkscreen for the card, but while looking for inspiration I found something that really caught my attention: exposed copper. At first it seemed easy to add to my own PCB, but all the tutorials I found were for older versions, and I couldn't find the option in the PCB editor. After a long time I realized it was in the image converter :( I felt really dumb at that moment.

<img width="720" height="418" alt="image" src="https://github.com/user-attachments/assets/bb59ccf2-414e-4d78-8244-e074dcf0d6f8" />

### October 3 - 40 min
After what happened a few hours earlier, I felt frustrated with myself, so I decided not to update the card as much as I originally wanted. Still, I knew it would be easy, and it was: adding a millimeter ruler to the back face of the PCB. After searching without success for an existing design online, I designed one quickly in Figma and hoped the measurements were accurate. In the end there was a small difference, but too small to really notice.

<img width="785" height="112" alt="image" src="https://github.com/user-attachments/assets/57b0b774-2434-4669-9580-11e9eff8a530" />

### October 4 - 40 min
Once the card itself was finished, it was time to set up the GitHub repository. Following the Expedition requirements, I added the production and original files to the repository. I also wrote the README.

### October 8 - 45 min
So after my project was required some changes, I had to get all the quota data from JCLPCB. I also had some issues on the way with the bom/csv files because they were broken in the last version due to some typos on them. Later I tried reducing the costs as much as possibke but couldnt find a way to get it below the $30 I was aiming for. I also edited the BOM in the description to have displayed all the quota data, added some more screenshots to the README and added a BOM.csv file directly from KiCad.

**Note: this all has been pushed on the same commit as I had the journals in a note on my mobile phone and just copy pasted it here.**
