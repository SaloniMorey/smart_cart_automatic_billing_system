# smart_cart_automatic_billing_system
A smart shopping cart prototype using ESP32, RFID, OLED/LCD displays, and a web interface. Automatically scans items, calculates bills in real time. Built for a seamless in-store shopping experience.

---

## 🚀 Features

- 📦 RFID-based Item Detection  
  Scan items using RFID tags to add or remove them from the cart.

- 🎛️ Add/Remove Buttons 
  Toggle between Add and Remove modes using hardware buttons.

- 🧾 Real-time Bill Calculation 
  Automatically updates total cost as items are added or removed.

- 📟 Dual Display Support 
  - OLED: Shows total and QR code for the bill.  
  - LCD: Displays scan status (e.g., "Item Added", "Item Removed", "Item Not Found").

- 🌐 Web Interface (ESP32-hosted)  
  - View cart contents live.  
  - Includes a Print Bill button 



## 🧰 Hardware Used

- ESP32 Dev Board (30-pin)
- MFRC522 RFID Reader
- RFID Tags
- OLED Display (128x64)
- I2C LCD Display (16x2)
- Push Buttons (Add / Remove / Show Total)
- Jumper Wires, and other supporting components

---

## 🛠️ Software Components

- **Arduino (C++)**
- Libraries Used:
  - MFRC522.h
  - LiquidCrystal_I2C.h
  - U8g2lib.h
  - WiFi.h
  - WebServer.h
- Custom code for:
  - Cart item management
  - LCD/OLED status display
  - Embedded web server (for real-time bill display)

## 🔧 Setup Instructions

### 1. Clone the Repository

bash
git clone https://github.com/SaloniMorey/smart_cart_automatic_billing_system.git
cd smart-cart


### 2. Install Required Libraries in Arduino IDE

Search for and install the following libraries via Library Manager:

* MFRC522
* LiquidCrystal\_I2C
* U8g2
* WiFi
* WebServer

### 3. Update WiFi Credentials

In the code, update your:

cpp
const char* ssid = "Your_SSID";
const char* password = "Your_PASSWORD";


### 4. Upload Code to ESP32

Use the correct COM port and board settings (ESP32 Dev Module) in Arduino IDE.
Upload the code and open Serial Monitor for debugging.

### 5. Access Web Interface

Once connected, the ESP32 will print its IP address.
Open that IP in a browser to view and print the bill.

---

## 📄 License

This project is open-source and available under the **MIT License**.
See the [LICENSE](LICENSE) file for more details.

---

## 🙌 Acknowledgments

* Inspiration from real-world checkout automation systems
* Libraries from the open-source Arduino community
* Project built as part of a hardware innovation challenge

```


