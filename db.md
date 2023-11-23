# Hospital Triage Database Design Documentation

## Entities Description

### Patients
Stores the individual patients in the triage system.

### Visits
Instances of a patient visiting our facility, whether by appointment or walk-in.

### Symptoms
Conditions reported which made a visit necessary. Recorded separately for each visit.

### Doctors
A list of medical personnel who can see patients.

### Rooms
A list of rooms to which patients can be assigned when a doctor is ready to see them.

## Attributes Specification

### Patients Attributes:
- patientID: automatically incremented surrogate key.
- healthCard: integer healthcard number, if present.
- versionCode: two letters at end of health card.
- dob: patient's date of birth. Included to differentiate patients who lack health cards.
- currentAddress: patient's address. Included to differentiate patients who lack health cards.

### Visits Attributes:
- visitID: automatically incremented surrogate key.
- patientID_fk: foreign key specifying which patient is visiting.
- doctorID_fk: foreign key specifying which doctor is assigned to this patient during this visit.
- roomID_fk: foreign key specifying which room the patient was sent to for this visit.
- arrivalTime: when the patient showed up and began waiting.
- seenByDoctor: when the patient was assigned a room/doctor.
- dischareTime: when the patient has been fully treated and is ready to leave.

### Symptoms Attributes:
-

### Doctors Attributes:

### Rooms Attributes:
-

## Database ERD (Entity-Relationship Diagram)
<!-- ![Database Schema](schema.png) -->

## Website Overview
This website will allow a patient to check in to the hospital and to input their symptoms and the location they feel pain into the hospital databse. A hospial worker will be able to look at the various patient's symptoms and will be able to decide who to treat first. 

## Design System

### Colour Palette
  -   **Text Colour:** '#000000' - The main text of on the website 
  -   **Backgroudnd Colour:** '#981d31' - Used for the colour of the main background 
  -   **Secondary Background Colour:** #555555' - Used for the colour of the any secondary backgrounds
  -   **Border Colour:** '#ffffff' - Border colour of tables and buttons
  -   **Header Colour:** '#6f7086' - Colour of the headers and titles
    
### Typography
- **Header Text:** '"Times New Roman", Times, serif'
- **Subheadings Text:** '"Times New Roman", Times, serif'
- **Body Text:** '"Times New Roman", Times, serif'

## Hospital Triage App Mock-Ups

## Patient Instructions
Patients will have to enter a piece of identification and then choose where their pain is and how bad the pain is. 

## Hospital Staff Instructions
Hospital Staff will go into the staff side of the webside and will see a list of patients that need help. The hospital staff will have to choose a patient that needs help and then go help them. When the patient has been seen, the staff member will have to remove that patient from the database. 

