# beacon.txt
Using the Arduino development environment, the ESP32 was programmed as a Line Simple Beacon device to enable short-range wireless communication. Through this application, the BLE (Bluetooth Low Energy) signals sent by the ESP32 are utilized in an interactive campus tour system at Soochow University’s Shuangxi Campus. The system leverages the BLE signals transmitted by the ESP32, allowing users to receive the signals via smartphones or other BLE-enabled devices and interact further with the campus tour system.
During the implementation process, we adopted the "ESP32 BLE Arduino" library to simplify development. The choice of Arduino as the development platform was driven by its intuitive interface, extensive community support, and high compatibility with the ESP32. Through a precise programming process, 10 ESP32 devices were sequentially named, corresponding to the HWIDs (Hardware Identifiers) applied for via the Line Official Account Manager. This ensured that each beacon accurately aligned with specific tour information at designated locations, enabling a complete interactive tour experience.
