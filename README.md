
# Student Enrollment Form Using JsonPowerDB

> A lightweight and efficient student enrollment form project using JsonPowerDB for backend database operations.
> 
---

## Table of Contents

- [Description](#description)
- [Benefits of using JsonPowerDB](#benefits-of-using-jsonpowerdb)
- [Scope of Functionalities](#scope-of-functionalities)
- [Examples of Use](#examples-of-use)
- [Installation](#installation)
- [Development Setup](#development-setup)
- [Project Status](#project-status)
- [Release History](#release-history)
- [Sources](#sources)
- [License](#license)

---

## Description

This project is a **Student Enrollment Form** developed using **HTML, Bootstrap, JavaScript**, and **JsonPowerDB**.  
It stores student data like Roll No, Full Name, Class, Birth Date, Address, and Enrollment Date securely in a database with fast retrieval, update, and delete functionalities.

The project demonstrates the practical use of JsonPowerDB's APIs in real-world dynamic applications.

---

## Benefits of using JsonPowerDB

-Simplest way to retrieve data in a JSON format.
-Schema-free, Simple to use, Nimble and In-Memory database.
-It is built on top of one of the fastest and real-time data indexing engine - PowerIndeX.
-It is low level (raw) form of data and is also human readable.
-It helps developers in faster coding, in-turn reduces development cost.
---

## Scope of Functionalities

- Add new student enrollment records.
- View existing student details by Roll No.
- Update existing student records.
- Reset form for new entries.
- Simple and clean Bootstrap 3 based UI.

---

## Examples of Use

Here’s a snippet of how you can store a new student record:

```javascript
var putReqStr = createPUTRequest(
  connToken,
  studentDataJson,
  "SCHOOL-DB",
  "STUDENT-TABLE"
);
executeCommandAtGivenBaseUrl(putReqStr, jpdbBaseURL, jpdbIML);
```

Retrieve student details using Roll No:

```javascript
var getReqStr = createGET_BY_KEYRequest(
  connToken,
  "SCHOOL-DB",
  "STUDENT-TABLE",
  studentRollNoJson
);
executeCommandAtGivenBaseUrl(getReqStr, jpdbBaseURL, jpdbIRL);
```

---

## Installation

1. Clone the repository:
```bash
git clone https://github.com/sohom2004/Login2Xplore-MicroProject.git
```
2. Open the `index.html` inside this folders:
   - `MicroProject/SiteRoot`

3. Make sure your internet connection is active (for Bootstrap and JPDB Commons script).

---

## Development Setup

To make changes:

- Update the HTML form fields as per need.
- Modify JavaScript for different DB operations.
- Customize JsonPowerDB connection credentials in the script.

---

## Project Status

> ✅ Completed basic functionalities for Student Enrollment with JsonPowerDB backend.  

---

## Release History

- **v1.0.0** (April 2025)
    - Initial Release
    - Features: Save, Update, Retrieve, Reset functionalities integrated with JsonPowerDB.
    - UI: Basic Bootstrap 3 styling.
    - Backend: Fully REST API driven using JsonPowerDB.

---

## Sources

- [JsonPowerDB Official Site](https://login2explore.com/)
- [Bootstrap Documentation](https://getbootstrap.com/)
- [jQuery Documentation](https://api.jquery.com/)

---

## License

Distributed under the MIT License. See `LICENSE` for more information.

---

> Made with ❤️ using JsonPowerDB and Bootstrap 3.
