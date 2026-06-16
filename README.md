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

<img width="997" height="523" alt="image" src="https://github.com/user-attachments/assets/0ce7ec04-7f43-4212-bf30-128ec8f2d939" />

## Wiring Plan

<img width="997" height="611" alt="image" src="https://github.com/user-attachments/assets/0e260511-e0fc-4b27-9d0a-ef80f4432d25" />

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
