# Security-and-log-iot-project---arduino
This is a security and log system of any organisaztion. 
ARDUINO UNO
RFID READER MFRC522
SERVO MOTOR
LCD SCREEN
LEDS

The rfid reader reads the card. The arduino sends the UID information to the python iterface using serial communication. Python code checks the presence of the UID in the student_info table. if present it checks whether the person is loggin in or not. If logging in, it inserts their information into the student_card table. If logging out it updates the log out time of that particular person. And if the UID is not present it says 'UID NOT FOUND' . It sends back the logging in or logging out or 'no uid' information to the arduino and it prints it on the LCD screen. There is also a voice module which announces the person's name and timpstamp using the GTTS and mixer module to convert the tect to audio file and play it.

  pinMode(4, OUTPUT); LED ONE RED- OF NO UID
  pinMode(5, OUTPUT); LED TWO GREEN- IF PERSON PRESENT 
  myservo.attach(6); SERVO MOTOR PIN
  LCD driver attcahed to A4 & A5
