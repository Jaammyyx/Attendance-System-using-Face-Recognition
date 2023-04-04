Attendance System using Face Recognition
This is a Python program that uses face recognition to take attendance of students in real-time using a webcam.

Installation
This program requires the following libraries to be installed:

cv2
face_recognition
numpy
csv
datetime
These can be installed using pip.

bash
Copy code
pip install opencv-python face_recognition numpy csv datetime
Usage
To use this program, run the following command:

bash
Copy code
python attendance.py
This will open up the webcam and start detecting faces. If a face matches a known face, the program will mark the student as present and record the time in a CSV file.

The CSV file will be named after the current date and will be created in the same directory as the program.

Press q to exit the program.

Configuration
Adding students
To add students to the attendance system, you need to add their images to the faces directory and update the known_faces_encoding and known_face_names variables in the code.

Changing the attendance file name
By default, the attendance file is named after the current date. If you want to change this, you can modify the current_date variable in the code.

Changing the text on the attendance window
You can modify the text that appears on the attendance window by updating the cv2.putText function in the code.

To modify the text that appears on the attendance window, you can update the parameters of the cv2.putText function in the code. Here is an explanation of the different parameters:

frame: The image frame on which the text will be displayed
name + " present": The text to be displayed on the frame
(10, 100): The coordinates of the bottom left corner of the text
cv2.FONT_HERSHEY_SIMPLEX: The font type of the text
1.5: The font scale of the text
(255, 0, 0): The font color in BGR format
3: The thickness of the text
2: The line type of the text
You can modify these parameters to customize the text that appears on the attendance window. For example, you can change the font type, font size, font color, and position of the text to match your requirements.

