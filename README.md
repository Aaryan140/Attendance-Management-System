Face Recognition Based Attendance System
A Python-based attendance system leveraging face recognition to mark attendance.

Overview
This project demonstrates an attendance system that employs face recognition to record attendance. The system is designed with a user-friendly graphical user interface (GUI) using Python's tkinter library, making it accessible and easy to use for anyone.

Technologies Used
tkinter: For the entire GUI.
OpenCV: For capturing images and performing face recognition using cv2.face.LBPHFaceRecognizer_create().
CSV, Numpy, Pandas, datetime: For various functionalities.
Key Features
User-friendly GUI: Easy to operate.
Password-protected registration: Ensures secure registration for new users.
Automatic CSV management: Creates and updates CSV files with student details upon registration.
Daily attendance logging: Generates a new CSV file each day for attendance, logging the date and time accurately.
Real-time attendance updates: Displays live attendance updates on the main screen, including ID, name, date, and time.
Prerequisites
Before you begin, ensure you have met the following requirements:

Python 3.x
The following Python libraries:
tkinter
OpenCV
numpy
pandas
PIL (Pillow)

Installation
Clone the repository:
git clone https://github.com/your-username/face-recognition-attendance-system.git
cd face-recognition-attendance-system


Install the required libraries:
pip install opencv-python-headless numpy pandas pillow


Ensure you have the Haar Cascade XML file for face detection:
Download it from OpenCV GitHub and place it in your project directory.

Usage
Run the script:
python attendance_system.py

Interface Overview:

For New Registrations:

Enter ID and Name.
Click on "Take Images" to capture images of the new user.
Click on "Save Profile" to save the profile (password-protected).
For Already Registered Users:

Click on "Take Attendance" to mark attendance using face recognition.
Password Management:

Change password from the "Help" menu by selecting "Change Password".
Contact information and exit options are also available in the "Help" menu.
Functions and Code Explanation
assure_path_exists(path): Ensures the directory exists, creates if not.
tick(): Updates the clock in the GUI.
contact(): Displays contact information.
check_haarcascadefile(): Checks if the Haar Cascade XML file exists.
save_pass(): Saves a new password.
change_pass(): Opens a window to change the password.
psw(): Prompts for the password to save the profile.
clear(): Clears the ID entry field.
clear2(): Clears the name entry field.
TakeImages(): Captures images of the new user for training.
TrainImages(): Trains the recognizer with the captured images.
getImagesAndLabels(path): Retrieves images and their corresponding labels from the specified path.
TrackImages(): Captures and recognizes faces to mark attendance.


Contact
For any inquiries or support, please contact: allentitiesdemise@gmail.com