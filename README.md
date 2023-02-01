# RFID Read/Write Test
#### Code taken and modified from https://www.instructables.com/ESP32-With-RFID-Access-Control/

## Testing
1. First wire up your microcontrolller:  
  - RFID SDA -> Arduino pin 53
  - RFID SCK -> Arduino pin 52
  - RFID MOSI -> Arduino 51
  - RFID MISO -> Arduino 50
  - RFID RST -> Arduino 49
  - RFID 3.3v -> Arduino 3.3v
  - RFID GND -> Arduino GND
  
2. Clone this repository's code into a new Arduino project.
3. Install the MFRC552 library for Arduino: https://github.com/miguelbalboa/rfid.
4. Upload the code to the Arduino
5. Open the Arduino IDE's serial monitor
### Reading the card data:
By default, the code only reads the data, so simply place your RFID card against the reader and view the results in the serial monitor

### Writing AND reading card data:
To put the code into write and read mode, change the `RFID_MODE` at the tip of the file to `1`.  
Then use the serial monitor input to choose whether to read or write. The card must remain on/near the reader when choosing an option or an error will occur)

