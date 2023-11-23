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


### Symptoms Attributes:

### Doctors Attributes:

### Rooms Attributes:
-

## Database ERD (Entity-Relationship Diagram)
<!-- ![Database Schema](schema.png) -->

T
