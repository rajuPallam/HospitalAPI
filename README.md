# HospitalAPI
      |
      |                |---mongoose.js
      |___config-------|---passport-jwt-strategy.js
      |
      |
      |                     |---doctor_controller.js
      |___controllers-------|---patient_controller.js
      |                     |---home_controller.js
      |                                                       |---doctor.js
      |___model-----------------------------------------------|---patient_report.js
      |                                                       |---patient.js
      |                  |---reports.js
      |__routes----------|---index.js
      |                  |---patient.js
      |                  |---doctor.js                       
      |                                                     
      |___.gitignore
      |
      |
      |___index.js
      |
      |
      |___package-lock.json
      |
      |
      |__package.json





                              **Features**
1.Doctor Registration and Login:
Doctors can register by providing a unique username and password.
Registered doctors can log in to the system using their credentials to access protected routes.

2.Patient Registration:
Patients can be registered in the system using their phone number.
If a patient with the provided phone number already exists, the API will return the patient's information.

3.Patient Report Creation:
After a patient visits, the doctor can create a report for the patient.
The report will include information such as the status (Negative, Travelled-Quarantine, Symptoms-Quarantine, Positive-Admit), the date of the report, and the doctor who created it.

4.JWT-Based Authentication:
The API uses JSON Web Tokens (JWT) to authenticate doctors for certain protected routes.
Upon successful login, the API will provide a JWT that the doctor can include in subsequent requests to access protected routes.

5.List All Reports of a Patient:
The API allows doctors to retrieve all reports of a specific patient, sorted from the oldest to the latest.
Each report will include information about the status, date, and the doctor who created it.

6.List All Reports Filtered by Status:
Doctors can retrieve a list of reports filtered by a specific status (e.g., Negative, Positive-Admit).
The API will return all the reports from different patients that match the specified status.

7.Scalable Folder Structure:
The project follows a scalable folder structure to separate concerns and make the codebase more organized and maintainable.
Controllers, models, and routes are separated, making it easier to add more features in the future.

8.Well-Commented Code:
The codebase is well-commented, providing explanations for important functions, routes, and logic.
This makes it easier for other developers to understand the code and collaborate on the project.

9.Error Handling:
Though not explicitly mentioned in the initial design, proper error handling should be implemented to handle various scenarios, such as invalid input, database errors, or server issues.
The API should return appropriate error responses with relevant status codes and error messages to guide the clients.
These features collectively provide a foundation for managing patient records, doctor authentication, and report creation for COVID-19 patients in the hospital. Depending on the specific requirements of the hospital and the application, additional features and functionalities can be added to enhance the API further.
