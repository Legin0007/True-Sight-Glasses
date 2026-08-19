## What this project does
This project looks at people's faces using a small camera attached to the glasses frame. If a face matches an entry in my repository, the system retrieves the file name and plays the audio through a small speaker into my ear. Also I would like to preface this by saying I am using a libary called ESP-WHO and the example code I am using is made by them and modified by me. Also here is the demo video https://youtube.com/shorts/fBa7BR6LM4Y?is=uIni2kENnGARo2fe
# Why I made this
This project was made because I have a poor memory and I often forget peoples names so this is a simple and semi-elegant solution.Other people that may use this are people with memory loss or other memory related illnesses or diseases. 
# Challenges I faced
When I was designing this I went through 3 versions of my build. The first design was replaced because the chip I was using was too big and ended up with 2 separate parts which wasn't optimal so I changed the chip and battery to be smaller and fit on one side but I had to change that because it wasn't compatible with the code so the final design uses a esp32-s3 Eye which led to it being wider than the 2nd design.
## Construction Instructions:
### Sourcing Parts
1.Download the BOM and open it in google sheets or some thing like it.
2.Go through all the links and buy the parts that are required.
3.Download the folder called "3D-Models" download them and print them using your respective slicer.
4.After you source all the parts put them in their respective positions and use the pins to hold them in place.
### Soldering parts
1.Solder the battery positive to B+ and the negative to the B-
2.Solder 2 wires to out- and 1 to out+
3.Solder the out+ wire to one side of the switch and solder 2 wires on the output of the switch
4.Solder one of the positive wires from the switch to the amp SD pin.
5.On the amp make a wire from Vin to SD along with the positive wire.
6.Solder from the amp BCLK to IO21 then then LRC to IO48 then DIN to IO47
7.Solder the one remaining positive and negative wire to the 2 + and - pins on the back of the esp32-s3 eye to provide power to that.
### Flashing the firmware
1.You need to download the folder labeled "Code".
2.Open VS code and go to file and select open folder then go to esp-who\examples\human_face_recognition and click open folder.
3.You need to install ESP-IDF from the link in Resources and select custom install then follow all the steps until it asks for the version which you select 5.5.4 and continue with the installation.
4.Go to VS code and install the ESP-IDF extension.
5.Press F1 and type  ESP-IDF: Open ESP-IDF Terminal then type idf.py reconfigure
6.Press F1 and type  ESP-IDF: Select Port to Use (COM, tty, usbserial)
7.Press F1 and run ESP-IDF: Build, Flash and Start a Monitor
8.Go to the file who_recognition.cpp then you need to find where it says "Hello Amma" and change it out with the first person you will enroll so on and so forth.
## Note
The parts are held in place by having a gap in the main body which is can be filled by a seperate pin which blocks the parts from moving.  
## Bom

| Name                     | Description                                     | Quanity | Unit Price | Shipping cost |
|--------------------------|-------------------------------------------------|---------|------------|---------------|
| Esp32s3-EYE              | Camera and for running the code                 | 1       | 45         | 0             |
| Lipo 3.7V 500mAh battery | For powering all parts of the project           | 1       | 8.59       | 3.26          |
| Bone Conduction Speaker  | To play peoples names                           | 1       | 2.16       | 0             |
| Adafruit Mono Amp        | gives the speaker instructions                  | 1       | 2.64       | 0             |
| On/Off Switch            | To enable and disable the power.                | 1       | 2.81       | 0             |
| 3.3v ldo regulator       | To make the volatage 3.3V                       | 1       | 1.85       | 0             |
| Soldering iron           | To attach wires to other parts                  | 1       | 2.75       | 0             |
| Solder                   | Melted metal to attach wires                    | 1       | 2.91       | 0             |
| Heatshrink Tubing        | Can cover wires for safety and looks            | 1       | 2.68       | 0             |
| Wires                    | To connect all electrical parts together        | 1       | 1.5        | 0             |
| Wire Stripper            | To remove plastic from wires for easy soldering | 1       | 3.43       | 0             |
| TP4056 charging module   | To recharge the battery                         | 1       | 5.99       | 0             |
| Total Cost               | The total cost of all items                     | 1       | 91.24      | 0             |


## Wiring Plan

<img width="1235" height="750" alt="image" src="https://github.com/user-attachments/assets/58532883-ece1-482b-ae92-df164af0bb3f" />

## Zine

<img width="483" height="683" alt="image" src="https://github.com/user-attachments/assets/1c11fc60-c8f2-4303-97d5-2b0e3df16a74" />

## Render

<img width="1920" height="632" alt="Nigels First numero 1" src="https://github.com/user-attachments/assets/752f37a6-fcee-442e-b914-9544da12ca63" />
<img width="1920" height="632" alt="True_Sight2" src="https://github.com/user-attachments/assets/b406203f-9311-4f8f-8269-89f5d115562c" />

## Cad

<img width="607" height="526" alt="image" src="https://github.com/user-attachments/assets/a4e24d69-5abc-4b90-9436-539e5fb3fccf" />
<img width="360" height="485" alt="image" src="https://github.com/user-attachments/assets/0d3d8b63-8ca1-4901-a49e-9768383e4f8d" />

## IRL Images

<img width="3024" height="4032" alt="WhatsApp Image 2026-08-18 at 8 24 54 PM (2)" src="https://github.com/user-attachments/assets/ffc99008-7db8-45f1-b3d6-82c887e37b67" />

<img width="4032" height="3024" alt="WhatsApp Image 2026-08-18 at 8 24 54 PM" src="https://github.com/user-attachments/assets/5aba24a6-9c00-4f0e-a27d-d0ded3ba35e1" />
<img width="577" height="433" alt="WhatsApp_Image_2026-08-18_at_8 24 54_PM-removebg-preview" src="https://github.com/user-attachments/assets/e31666d1-6062-494b-87bd-4f4b1840d8b7" />

## Resources

Download link 
https://docs.espressif.com/projects/idf-im-ui/en/latest/
ESP-WHO link 
https://developer.espressif.com/blog/2026/05/esp-who-get-started/
