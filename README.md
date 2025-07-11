#   Damage Demarcation in Post-Disaster Scenarios

A Python-based client-server framework designed to automate the detection, classification, and demarcation of structural damage from post-disaster images (e.g., earthquakes). This system simulates drones (clients) sending images to a central server, which then analyzes and classifies the damage using image processing and machine learning techniques.

---

##   Table of Contents

-  Objective 
-  Key Features 
-   Folder Structure 
-  Technologies Used 
-  Setup & Execution 
-  Sample Results 
-  Future Enhancements 
-  Author 
-  License 

---

##   Objective

In the aftermath of natural disasters such as earthquakes, timely and accurate structural damage assessment is critical for rescue and rebuilding efforts. Manual inspection is dangerous and time-consuming. This project enables:
- Drone-based image capture
- Real-time server-side damage classification
- Automated demarcation and visual output
- Scalable multi-drone support

---

##  Key Features

 **Multi-threaded Server**: Accepts multiple drone image streams simultaneously  
 **Client-Server Communication**: Uses TCP sockets for robust, real-time transfer  
 **Damage Classification**: Applies image processing techniques (OpenCV) to identify cracks, breaks, and other damage patterns  
 **Visual Output**: Saves processed images with damage boundaries marked  
 **Storage and Logging**: Automatically stores outputs and logs communications  
**Lightweight Design**: Suitable for deployment on edge devices with limited resources

---

##  Folder Structure

├── server/ # Server-side logic
│ ├── server.py # Main socket server
│ ├── image_processor.py # Image processing & demarcation
│ ├── classifier.py # Classification logic
│ └── utils.py # Helper functions
├── client/ # Client (drone simulator)
│ └── client.py # Image sender
├── processed_images/ # Output with damage marked
├── requirements.txt # Python dependencies
└── README.md # Project documentation

