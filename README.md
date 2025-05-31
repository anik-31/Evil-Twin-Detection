# Evil Twin Detection

This repository contains the implementation of an **Evil Twin Detection System** using an **ESP32** microcontroller and a **Random Forest Classifier**. The system scans Wi-Fi networks in the environment, classifies them as legitimate or malicious (Evil Twin), and displays the results in real-time using a **Streamlit dashboard**.

---

## Features

- **Wi-Fi Scanning**:
  - Detects nearby Wi-Fi networks and retrieves information such as SSID, BSSID, RSSI, channel, and encryption type.
  
- **Classification**:
  - Uses a pre-trained Random Forest Classifier to identify malicious Evil Twin networks.

- **Real-Time Visualization**:
  - Displays classification results dynamically in a Streamlit dashboard.

- **Custom Dataset**:
  - Built a dataset of legitimate and simulated Evil Twin networks for model training and testing.

---

## Installation

### Prerequisites

1. **Hardware**:
   - ESP32 (e.g., ESP32 WROVER-IB)

2. **Software**:
   - Python 3.8 or above
   - Anaconda (optional, for managing environments)
   - PlatformIO for ESP32 programming

3. **Libraries**:
   - Install required Python libraries:
     ```bash
     pip install -r requirements.txt
     ```

### Setting Up

1. Clone the repository:
   ```bash
   git clone https://github.com/anik-31/Evil-Twin-Detection.git
   cd Evil-Twin-Detection
   ```

2. Upload the ESP32 code (from the `ESP32_Code` folder) to the ESP32 using PlatformIO or Arduino IDE.

3. Start the Streamlit dashboard:
   ```bash
   streamlit run dashboard.py
   ```

---

## Usage

1. Power up the ESP32.
2. Connect the ESP32 to your machine via USB or serial.
3. Run the Streamlit dashboard.
4. View real-time network classifications as the ESP32 scans and sends Wi-Fi data.

---

## Project Structure

```
Evil-Twin-Detection/
├── ESP32_Code/              # Code for Wi-Fi scanning on ESP32
├── Dataset/                 # Dataset for training the Random Forest Classifier
├── Models/                  # Pre-trained machine learning models
├── dashboard.py             # Streamlit dashboard for visualization
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```

---

## Results

- **Model Accuracy**: Achieved 95% accuracy in distinguishing Evil Twin networks from legitimate ones.
- **Real-Time Detection**: Successfully detects and classifies networks in under 2 seconds.

---

## Technologies Used

- **Hardware**: ESP32
- **Programming Languages**: Python, Embedded C
- **Machine Learning**: Random Forest Classifier
- **Visualization**: Streamlit Dashboard

---

## Future Work

- Extend support for additional machine learning models.
- Integrate a cloud-based dashboard for remote monitoring.
- Enhance dataset with more real-world Evil Twin examples.

---

## Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request.

---

---

## Contact

For questions or suggestions, please contact **anik-31** via [GitHub Issues](https://github.com/anik-31/Evil-Twin-Detection/issues).
