# Setting Up

Before we do anything, you will need to set up your IDE.
Your IDE is where we will write our code and upload code to the microcontrollers.

## Setting Up ArduinoIDE

### Desktop Editor
- Open the microsoft store
- Search for Arduino IDE
- Download

1. ![Open the Microsoft Store](https://github.com/user-attachments/assets/3e1e9c03-de14-4d4d-a4fb-ad7c69c11293)
2. ![Search for Arduino IDE](https://github.com/user-attachments/assets/ef63ef11-fee8-4fd1-848d-80ea0898a8b2)

#### Setting Up ESP-32 Development
The Arduino IDE can work with any Arduino boards straight after download with no extra work. These boards include Arduino Uno, Nano, Mega and more.

However, we will be working with third-party boards called ESP-32's. These work very similar, but we will still need to download some extra libraries to the IDE so that the Arduino IDE can communicate with our boards.

- Open Arduino IDE
- Click the "Tools" dropdown from the menu at the top
- Open the "Board" dropdown menu and click "Board Manager"
- Search for "esp32" and download the library by Espressif Systems (**N.B.** dont install the library called "Arduino ESP32 Boards", make sure to install the library called "esp32")

1. ![Tools dropdown](https://github.com/user-attachments/assets/542590ae-c39b-495b-b1c3-ab02a8b13e48)
2. ![Download esp32 library](https://github.com/user-attachments/assets/e4fdfd47-e984-4291-8820-f01ec936295e)

#### Installing USB Drivers
For the PC to upload code to the Arduino's, we will need to install a driver to tell the computer how to talk to the Arduino's.
- Go to [Silicone Labs download page](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads)
- Download the Universal Windows Driver
- Find where you downloaded the driver on your PC (This will usually be in the Downloads folder)
- Unzip the folder

- Search for Device Manager in the start tab
- Find the device that says USB to UART
- Right click and select Update Drivers
- Click browse my computer for drivers
- Select the folder you unzippes and select it

  ![image](https://github.com/user-attachments/assets/eaa538b2-6849-4429-828b-8567a4674837)
  ![image](https://github.com/user-attachments/assets/27a81e5a-df5f-4741-8d05-c8c70be89caf)
  ![image](https://github.com/user-attachments/assets/141d5d5b-70d5-4996-9e35-ef7bab4f0751)


  

