# User-Interface-to-Control-a-Robot-Arm

Downloading and Installing The Interface Package Steps:
  1. Download XAMPP.
  2. Start Apache & MySQL from XAMPP.
  3. Save the Interface package in this path: C:\xampp\htdocs.
  4. Create the database (Steps mentioned in the creation process bellow "step 4"). 
  5. Open a browser and enter localhost/interface/index.html.
  6. Press on (تحفظ) to save the entered values to the database.
  7. Press on (تشغيل) to extract the last row saved from the database and change the On_Mode column to "on".

Creation Process:
  1. Download Virtual Studio Code.
  2. Build the website's main component with HTML (index.html). It includes a range input, a label, and a text input for each motor. Two buttons are also included to send the data to the database (تحفظ), and to run the motors (تشغيل) when connected to ROS. 
  3. Design the user interface with CSS (style.css).
  4. Create a database called "Motors" with eight columns (id, Motor 1, Motor 2, Motor 3, Motor 4, Motor 5, Motor 6, On_Mode) on phpMyAdmin. id is an AutoIncrement Int(1000), Motor # are an Int(11), and On_Mode is a Varchar(11) that is Null by default.
  5. Connect to the database and display the motors' degree on a PHP page (results.php).  This page will run when the user clicks on the save (تحفظ) button. 
  6. Extract the last row saved from the database and display the results on a PHP page (run.php). Additionally, Chane the On_Mode column to "on" in the extracted column. This page will run when the user clicks on the run (تشغيل) button. 
