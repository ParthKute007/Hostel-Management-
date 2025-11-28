# Hostel Management System
  A robust, Python-based desktop application designed to modernize and streamline the day-to-day administrative operations of managing a hostel. This system digitizes the entire workflow, handling room              allocation,  student admission, and real-time vacancy tracking using a lightweight, file-based storage approach. By utilizing JSON for data persistence, the application eliminates the need for complex database     servers,        making it highly portable and easy to run on any standard computer.
## Key Features
 •	Intelligent Room Allocation Logic: The system enforces strict capacity constraints. Before confirming a student's admission, the application checks the specific room's current occupancy against its maximum      capacity to prevent double-booking.
 •	Secure Admin Panel: Includes a password-protected administrative view (Password: 3939) that allows authorized staff to view the complete list of all registered students along with their specific Admission IDs   for easy reference.
 •	Comprehensive Student Database: Acts as a centralized repository for all resident information, storing Student Name, Unique ID, Contact Phone Number, and Admission Date.
 •	Dynamic Vacancy Tracking: The application maintains a real-time count of available beds. The vacancy count decreases upon registration and increases immediately when a student checks out.
 •	Zero-Config Data Persistence: Data integrity is maintained through a local hostel_data.json file. The system serializes all objects to JSON, ensuring records remain intact even after the application is closed.
 Technologies & Design Rationale
 •	Language: Python 3.x - Selected for its readability and extensive standard library.
 •	Storage Strategy: JSON - Chosen for maximum portability and zero-installation requirements.
 •	User Interface: CLI (Command Line Interface) - Ensures the application is lightweight and distraction-free.
## Modular Project Structure
 The codebase adheres to the Single Responsibility Principle:
 •	DataManager: Handles safe loading and saving of the JSON file.
 •	RoomManager: Manages room inventory and capacity logic.
 •	StudentManager: Handles student registration, ID generation, and the new Admin view.
## Steps to Install & Run
 1.	Clone the Repository
 2.	Navigate to Directory:
 3.	cd hostel-management-system
 4.	Run the Application:
 5.	python main.py
## Detailed Instructions for Testing
 To verify the system's robustness, perform the following test scenarios:
 ### Scenario A: The Happy Path
 1.	Add a Room: Select option 1. Create Room #101 with a Capacity of 2.
 2.	Register Student: Select option 3. Enter Name "as you like" and assign to Room #101.
 3.	Check Availability: Select option 2. Verify that Room #101 now shows "1/2" occupancy.
 ### Scenario B: Admin Access Test
  1.	Select Admin View: Choose option 6 from the main menu.
  2.	Enter Password: Type (3939) when prompted.
  3.	Verify Output: Ensure a list of all students (IDs and Names) is displayed.
  4.	Security Check: Try option 6 again with a wrong password and verify access is denied.
 ### Scenario C: Data Persistence
  1.	Restart App: Close the terminal and run python main.py again.
  2.	Verify Data: Check if the student "John Doe" still exists in the system.




































