# Student Result Management System (SRMS)

## SDLC Model Used
Waterfall Model
 
 1. Requirement Analysis
The system is designed to manage student results.

  Functional Requirements
- Add student details
- Add student results
- View student results

  Non-Functional Requirements
- Easy to use
- Fast performance
- Secure data storage

---

  2. System Design

  Architecture
The system uses a three-tier architecture:
- Presentation Layer (HTML)
- Application Layer (Python Flask)
- Database Layer (SQLite)

   Database Design

  Student Table
- id
- name
- matric_number

 Result Table
- id
- student_id
- course
- score

 3. Implementation
The system is implemented using:
- Python
- Flask
- SQLite
- HTML

 4. Testing
System testing was carried out to ensure all features work correctly.

 5. Deployment
The application is deployed locally using Flask development server.

 6. Maintenance
Future improvements include:
- User authentication
- Better UI design
