**assignment_portal** 

Overview

The Assignment Portal is a backend system designed to handle assignment submissions.
It allows users to upload assignments and enables admins to manage them (accept or reject). The system is built using Flask and MongoDB.


**Features**
**User Functionalities:**

Register and log in.

Upload assignments.

View available admins.

**Admin Functionalities:**

Register and log in.

View assignments assigned to them.

Accept or reject assignments.

**Authentication:**

Secure JWT-based authentication for all endpoints.

**API Endpoints**

**User Endpoints**

POST /user/register: Register a new user.

POST /user/login: Log in as a user.

POST /user/assignment/upload: Upload an assignment.

GET /user/admins: Fetch the list of admins

**Admin Endpoints**

POST /admin/register: Register a new admin
.
POST /admin/login: Log in as an admin.

GET /admin/<admin_id>/assignments: View assignments tagged to an admin.

POST /admin/<admin_id>/assignments/<assignment_id>/accept: Accept an assignment.

POST /admin/<admin_id>/assignments/<assignment_id>/reject: Reject an assignment.

**Testing**

Use a tool like Postman or cURL to test the endpoints.

Ensure valid JWT tokens are included in the headers for protected endpoints.

**Access the app at http://localhost:5000.**

