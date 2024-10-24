# IOT-PROJECT-SMART ALGARICULTURE FARM 

### Key Components of the Code

1. **Libraries and Definitions**:
   - `#define BLYNK_PRINT Serial`: This allows Blynk to print debug messages to the Serial Monitor.
   - `#include <ESP8266WiFi.h>`: Includes the ESP8266 Wi-Fi library to enable Wi-Fi capabilities.
   - `#include <BlynkSimpleEsp8266.h>`: Includes the Blynk library for ESP8266.

2. **Credentials**:
   - The code stores the Blynk authentication token, Wi-Fi SSID, and password in character arrays.

3. **Setup Function**:
   - Initializes serial communication.
   - Configures the water pump pin as an output and sets it to LOW (off).
   - Connects to the Blynk server using the provided credentials.
   - Sets a timer to periodically call the `soilMoistureSensor` function.

4. **Blynk Control**:
   - `BLYNK_WRITE(V1)`: A callback function triggered by a virtual button in the Blynk app. It controls the water pump based on user input.

5. **Soil Moisture Sensing**:
   - The `soilMoistureSensor` function reads analog values from a soil moisture sensor, maps the raw values to a percentage, and sends this data to the Blynk app.

6. **Loop Function**:
   - Calls `Blynk.run()` to process Blynk tasks and `timer.run()` to manage the Blynk timer.

### Key Features
- **Remote Monitoring**: The system can monitor soil moisture levels and control a water pump remotely via a Blynk app.
- **Real-Time Feedback**: The moisture levels are displayed in the app, allowing users to see the moisture percentage in real-time.
- **Automated Control**: The water pump can be manually turned on or off from the app.

### Summary
This code demonstrates a practical application of IoT (Internet of Things) using C++ for microcontrollers, integrating hardware components with cloud services for smart plant management.





![gambar team 9](https://github.com/NurulAthira26/IOT-PROJECT-GROUP-9/assets/93875055/8e9d0bae-38cf-4cf5-8ab1-d32364243440)
![gambar iot](https://github.com/NurulAthira26/IOT-PROJECT-GROUP-9/assets/93875055/51203fdd-8344-4950-b622-d62a9e01c89f)
![project iot](https://github.com/NurulAthira26/IOT-PROJECT-GROUP-9/assets/93875055/6adac4ac-2e6d-48ab-9b3b-f324d33bf814)
