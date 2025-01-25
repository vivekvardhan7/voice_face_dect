# Voice and Face Detection System

This project is a real-time detection system designed to track voice activity and facial features. It aims to assist in scenarios such as online proctoring, security monitoring, and user verification. By detecting multiple voices and monitoring face and eye movements, the system helps identify unusual activities or unauthorized presence, ensuring integrity in monitored environments.

## Features

- **Dual Voice Detection**:
  - Utilizes WebRTC's Voice Activity Detection (`webrtcvad`) to identify multiple voices.
  - Detects unauthorized background sounds.

- **Face and Eye Tracking**:
  - Leverages OpenCV’s Haar Cascade classifiers to detect faces and eyes.
  - Tracks facial and eye positions in real-time.

- **Real-Time Alerts**:
  - Provides live feedback on detected activities.
  - Highlights issues like multiple voices or unusual eye movements, indicating potential cheating or unauthorized presence.

- **User Interface**:
  - Simple GUI built with `tkinter`.
  - Displays the video feed and detection alerts for user-friendly interaction and visualization.

## Technology Stack

### Audio Processing
- **Libraries**: `pyaudio`, `webrtcvad`

### Computer Vision
- **Libraries**: `opencv-python`

### GUI Framework
- **Framework**: `tkinter`
- **Image Rendering**: `Pillow`

## Installation Requirements

### General Requirements
- Python 3.7+
- Libraries:
  - `pyaudio`
  - `webrtcvad`
  - `opencv-python`
  - `numpy`
  - `Pillow`
  - `tkinter` (included with Python on most systems)

### Additional Requirements for Windows
Some dependencies may require additional setup tools:

- **CMake**: Required to build certain packages on Windows.
- **dlib** (optional): Installable via `pip` for extended face feature tracking. Note: This is not mandatory for basic functionality.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/voice-face-dect-system.git
   cd voice-face-detection-system
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. For Windows users, ensure `cmake` is installed. You can install it using `pip`:
   ```bash
   pip install cmake
   ```

4. (Optional) For extended face tracking, install `dlib`:
   ```bash
   pip install dlib
   ```

## Usage

1. Run the main script:
   ```bash
   python main.py
   ```

2. The application will launch with a GUI displaying the video feed and detection alerts.

3. Follow the on-screen instructions to monitor and analyze activities in real time.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue to discuss changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [WebRTC Voice Activity Detection (webrtcvad)](https://github.com/wiseman/py-webrtcvad)
- [OpenCV](https://opencv.org/)
- [Python Pillow Library](https://python-pillow.org/)

---

**Note**: Ensure your system supports the required libraries and dependencies before installation.
****
