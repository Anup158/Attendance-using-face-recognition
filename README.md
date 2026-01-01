# 🤖 Attendance System using Face Recognition

<div align="center">

[![GitHub stars](https://img.shields.io/github/stars/Anup158/Attendance-using-face-recognition?style=for-the-badge)](https://github.com/Anup158/Attendance-using-face-recognition/stargazers)

[![GitHub forks](https://img.shields.io/github/forks/Anup158/Attendance-using-face-recognition?style=for-the-badge)](https://github.com/Anup158/Attendance-using-face-recognition/network)

[![GitHub issues](https://img.shields.io/github/issues/Anup158/Attendance-using-face-recognition?style=for-the-badge)](https://github.com/Anup158/Attendance-using-face-recognition/issues)

[![GitHub license](https://img.shields.io/github/license/Anup158/Attendance-using-face-recognition?style=for-the-badge)](LICENSE) <!-- TODO: Add a LICENSE file if open-source -->

**An automated attendance system leveraging real-time face detection and recognition.**

</div>

## 📖 Overview

This project provides a robust solution for automated attendance management using state-of-the-art face recognition technology. It's designed to stream video from a webcam, detect human faces, and accurately identify known individuals to mark their attendance. The system timestamps each attendance record and stores it persistently, making it an efficient tool for schools, offices, or events.

## ✨ Features

-   **Real-time Face Detection:** Automatically identifies and locates faces within a live webcam feed.
-   **Accurate Face Recognition:** Compares detected faces against a database of registered individuals to verify identity.
-   **Automated Attendance Marking:** Records the presence of recognized individuals without manual intervention.
-   **Timestamped Records:** Logs attendance with precise date and time information.
-   **CSV Export:** Stores all attendance data in a user-friendly CSV file for easy access and analysis.
-   **Easy Setup & Execution:** A standalone Python script designed for straightforward deployment.

## 🛠️ Tech Stack

**Core Technologies:**
-   ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

**Libraries:**
-   ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white) (for image processing and webcam interaction)
-   ![Face Recognition](https://img.shields.io/badge/Face_Recognition-4285F4?style=for-the-badge&logo=tensorflow&logoColor=white) (specifically the `face_recognition` library for Python)
-   ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white) (for numerical operations, often a dependency of OpenCV and face_recognition)

**Data Storage:**
-   CSV Files

## 🚀 Quick Start

Follow these steps to set up and run the attendance system on your local machine.

### Prerequisites

Before you begin, ensure you have the following installed:

-   **Python 3.x** (preferably 3.7 or newer)
-   A working **webcam**

### Installation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/Anup158/Attendance-using-face-recognition.git
    cd Attendance-using-face-recognition
    ```

2.  **Prepare the code**
    The core logic is currently in `complete code.txt`. For proper execution as a Python script, rename it:
    ```bash
    mv "complete code.txt" attendance_system.py
    ```

3.  **Install dependencies**
    Install the required Python packages using `pip`. It is recommended to use a virtual environment.
    ```bash
    # (Optional) Create and activate a virtual environment
    python -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate

    # Install packages
    pip install opencv-python face-recognition numpy
    ```

4.  **Prepare Known Faces**
    The `face_recognition` library needs known faces to compare against. You'll typically create a `faces/` directory (or similar) at the root of your project and place images of individuals you want the system to recognize inside it.
    
    *Example Directory Structure for Known Faces:*
    ```
    Attendance-using-face-recognition/
    ├── attendance_system.py
    ├── faces/
    │   ├── person_a.jpg
    │   ├── person_b.png
    │   └── ...
    └── (other project files)
    ```
    
    The `attendance_system.py` script will likely encode these faces when it first runs or on demand. **Please inspect the `attendance_system.py` file to understand how it expects known faces to be provided or registered.**

### Usage

1.  **Run the attendance system script**
    Navigate to the project directory in your terminal and execute the main Python script:
    ```bash
    python attendance_system.py
    ```
    
    This will typically activate your webcam feed. As faces appear, the system will attempt to recognize them and log attendance.

2.  **Monitor Attendance Records**
    Attendance records will usually be saved in a CSV file (e.g., `attendance.csv`) in the same directory as the script. You can open this file with any spreadsheet software to view the logged attendance.

## 📁 Project Structure

```
Attendance-using-face-recognition/
├── COMPLETE REPORT FINAL 1.docx   # Detailed project report
├── PBL FINAL PPT.pptx             # Project presentation slides
├── attendance_system.py           # Main Python script (originally complete code.txt)
├── faces/                         # TODO: Create this directory and add images of known individuals for recognition
└── attendance.csv                 # TODO: This file will be generated automatically upon first attendance record
```

## ⚙️ Configuration

The `attendance_system.py` script might contain hardcoded configurations or parameters that can be adjusted:

-   **Known Faces Directory:** The path where images of known individuals are stored (e.g., `faces/`).
-   **Attendance Log File:** The name of the CSV file where attendance records are saved (e.g., `attendance.csv`).
-   **Recognition Thresholds:** Parameters controlling the sensitivity of face recognition.

**Please review the `attendance_system.py` file directly for any configurable variables or parameters.**

## 🤝 Contributing

We welcome contributions to improve this attendance system!

1.  **Fork the repository.**
2.  **Create a new branch** for your feature or bug fix: `git checkout -b feature/your-feature-name`.
3.  **Make your changes** and ensure they are well-documented and tested.
4.  **Rename `complete code.txt` to a proper `.py` file** if it's still named `.txt` in your fork and submit your contributions in `.py` format.
5.  **Commit your changes:** `git commit -m 'feat: Add new feature X'`.
6.  **Push to your branch:** `git push origin feature/your-feature-name`.
7.  **Open a Pull Request** to the `main` branch of this repository.


## 🙏 Acknowledgments

-   **[Anup158](https://github.com/Anup158)** for initiating this project.
-   The developers of the `face_recognition` and `OpenCV` libraries for providing powerful tools for computer vision tasks.

## 📞 Support & Contact

-   🐛 Issues: [GitHub Issues](https://github.com/Anup158/Attendance-using-face-recognition/issues)
- jagtapanup158@gmail.com

---

<div align="center">

**⭐ Star this repo if you find it helpful!**

Made with ❤️ by [Anup158](https://github.com/Anup158)

</div>

