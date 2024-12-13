# Video Example
### https://youtu.be/zfCnd4RdNok

# beacon.txt
### Using the Arduino development environment, the ESP32 was programmed as a Line Simple Beacon device to enable short-range wireless communication. Through this application, the BLE (Bluetooth Low Energy) signals sent by the ESP32 are utilized in an interactive campus tour system at Soochow University’s Shuangxi Campus. The system leverages the BLE signals transmitted by the ESP32, allowing users to receive the signals via smartphones or other BLE-enabled devices and interact further with the campus tour system.
### During the implementation process, we adopted the "ESP32 BLE Arduino" library to simplify development. The choice of Arduino as the development platform was driven by its intuitive interface, extensive community support, and high compatibility with the ESP32. Through a precise programming process, 10 ESP32 devices were sequentially named, corresponding to the HWIDs (Hardware Identifiers) applied for via the Line Official Account Manager. This ensured that each beacon accurately aligned with specific tour information at designated locations, enabling a complete interactive tour experience.

# main.ipynb
### After completing the HWID (Hardware Identifier) configuration for the beacons, we used Flask in conjunction with the Line Bot API to enable interaction between the beacons and the Line Bot. The core of the system utilizes Flask's Webhook functionality to receive event requests from Line. When a user approaches a beacon and triggers HWID transmission, the Webhook identifies the event type, queries the corresponding campus tour content from the database based on the HWID, and delivers the relevant content to the user in real-time, achieving an interactive tour experience.
### To enhance the interactive experience, we implemented Carousel Template and Image Template designs for message responses. The Carousel Template provides a multi-card carousel with text and image options, where each card includes a title, image, and buttons that guide users to explore more details or external resources. The Image Template displays a preview video of the tour location, allowing users to click and watch, enriching the visual aspect of the campus tour. These templates, combined with multimedia presentations, offer users a more engaging and interactive campus tour experience.
### Additionally, the system design integrates HWID with the campus tour database to ensure efficient message queries. The Flask application was deployed on the Render platform to provide stable Webhook services. Furthermore, the video carousel feature enhances interactivity, enabling users to quickly browse campus tour videos. The overall design seamlessly integrates the beacon with the Line Bot, delivering an intuitive and vivid tour experience to users.

# ngrok.ipynb
### Process IP.

# requirements.txt
### Install all the packages we need.

# Additional information
### Our goal is to let everybody know our campus at anytime and easily
### Line is a communication app similar to Messages, and it is popular in Korea, Taiwan and Japan.
