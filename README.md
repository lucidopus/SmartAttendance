# Attendance Management System

This Attendance Management System utilizes facial recognition technology to streamline the process of tracking attendance in educational institutions. The system captures real-time images of students via webcam, recognizes their faces, and logs their attendance along with the relevant class details into a CSV file.

## Features

- **Real-time Face Recognition**: The system uses the `face_recognition` library to identify registered students through their webcam feed.
- **Automated Attendance Logging**: Attendance records are automatically created in CSV format, including the student's name, time of attendance, subject, teacher, and remarks on attendance status.
- **Daily Class Schedule Management**: The system reads a timetable from a CSV file to determine which subject is currently being taught and who the respective teacher is.
- **User-Friendly Webcam Interface**: A simple HTML interface allows teachers or administrators to take pictures using the webcam.

## Getting Started

### Prerequisites

- Python 3.x
- Libraries: `opencv-python`, `face_recognition`, `numpy`, `pandas`, `csv`
- A CSV file named `timetable.csv` containing the schedule of classes.
- A folder named `RegisteredCandidates` containing images of registered students for face recognition.

### Installation

1. Clone this repository or download the source code.
2. Install the required libraries using pip:
```bash
pip install opencv-python face_recognition numpy pandas
```

3. Ensure you have the images of students stored in the `RegisteredCandidates` directory.
4. Create a `timetable.csv` file formatted with class times and subjects for each day of the week.

## Usage

1. Run the main script that implements the facial recognition and attendance tracking functionality.
2. The system will access the webcam and begin scanning for registered students.
3. When a student is recognized, their attendance will be logged automatically.

## HTML Interface

An HTML interface is provided to allow users to capture images via a webcam. The code is structured to attach the webcam to a specified area on the page, and users can take snapshots that are displayed in the browser.

## References

- [OpenCV](https://opencv.org/) for image processing capabilities.
- [face_recognition](https://github.com/ageitgey/face_recognition) for face recognition functionality.
- [pandas](https://pandas.pydata.org/) for data manipulation and analysis.
