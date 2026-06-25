## What this project does
This project looks at people's faces using a small camera attached to the glasses frame. If a face matches an entry in my repository, the system retrieves the file name and plays the audio through a small speaker into my ear. Also I would like to preface this by saying I am using a libary called ESP-WHO and the example code I am using is made by them and modified by me.
# Why I made this
This project was made because I have a poor memory and I often forget peoples names so this is a simple and semi-elegant solution.Other people that may use this are people with memory loss or other memory related illnesses or diseases. 

## Construction Instructions:
### Sourcing Parts
1.Download the BOM and open it in google sheets or some thing like it.
2.Go through all the links and buy the parts that are required.
3.Download the folder called "3D-Models" download them and print them using your respective slicer.
### Flashing the firmware
1.You need to download the folder labeled "Code".
2.Open VS code and go to file and select open folder then go to esp-who\examples\human_face_recognition and click open folder.
3.You need to install ESP-IDF from the link in Resources and select custom install then follow all the steps until it asks for the version which you select 5.5.4 and continue with the installation.
4.Go to VS code and install the ESP-IDF extension.
5.Press F1 and type  ESP-IDF: Open ESP-IDF Terminal then type idf.py reconfigure
6.Press F1 and type  ESP-IDF: Select Port to Use (COM, tty, usbserial)
7.Press F1 and run ESP-IDF: Build, Flash and Start a Monitor
8.Go to the file who_recognition.cpp then you need to find where it says "Hello Amma" and change it out with the first person you will enroll so on and so forth.
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
| Total Cost               | The total cost of all items                     | 1       | 81.87      | 0             |


## Wiring Plan

<img width="1235" height="750" alt="image" src="https://github.com/user-attachments/assets/58532883-ece1-482b-ae92-df164af0bb3f" />

## Zine

<img width="1545" height="2000" alt="1" src="https://github.com/user-attachments/assets/ec55c3d2-3d21-426c-b23b-758087df9d74" />

## Render

<img width="1920" height="632" alt="Nigels First numero 1" src="https://github.com/user-attachments/assets/752f37a6-fcee-442e-b914-9544da12ca63" />
<img width="1920" height="632" alt="True_Sight2" src="https://github.com/user-attachments/assets/b406203f-9311-4f8f-8269-89f5d115562c" />

## Resources

Download link 
https://docs.espressif.com/projects/idf-im-ui/en/latest/
ESP-WHO link 
https://developer.espressif.com/blog/2026/05/esp-who-get-started/
