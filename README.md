# Face_Recognition_Based_Attendance_System

A python GUI integrated attendance system using face recognition to take attendance.

In this python project, I have made an attendance system which takes attendance by using face recognition technique. I have also intergrated it with GUI (Graphical user interface) so it can be easy to use by anyone. GUI for this project is also made on python using tkinter.

TECHNOLOGY USED:
1) tkinter for whole GUI
2) OpenCV for taking images and face recognition (cv2.face.LBPHFaceRecognizer_create())
3) CSV, Numpy, Pandas, datetime etc. for other purposes.

# Key Features:

1) Password Management:
        Allows setting, updating, and verifying passwords stored in a text file (psd.txt).

2) User Registration:
        Facilitates capturing facial images for new users.
        Stores images in the TrainingImage directory.
        Saves user details (ID and name) in a CSV file.

4) Face Recognition:
        Uses the Local Binary Patterns Histogram (LBPH) algorithm to train the system for recognizing faces.
        Trained data is saved as Trainner.yml.

5) Attendance Tracking:
        Recognizes faces using the webcam.
        Marks attendance in a CSV file (Attendance_<date>.csv) with details like date and time.

6) Graphical User Interface (GUI):
        Built using Tkinter with frames, buttons, and labels.
        Displays attendance logs using a TreeView widget.
        Provides options to register new users, take attendance, and manage passwords.

7) Utility Functions:
        assure_path_exists: Ensures required directories exist.
        check_haarcascadefile: Verifies the presence of the Haar cascade XML file.
        tick: Updates the clock displayed in the GUI.
        contact: Displays contact information.


# How It Works:

1) GUI Setup:

    The main window contains two frames for:
    New user registration.
    Attendance tracking for existing users.

2) New User Registration:

    Users enter their ID and name.
    The system captures facial images and stores them in TrainingImage.
    Profile is saved by training a facial recognizer model.

3) Taking Attendance:

    Captures live video feed.
    Detects faces in the feed.
    Matches faces with the trained model and logs attendance.

4) TreeView Display:

    Displays a list of users and their attendance information in the GUI.
