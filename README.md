# QA Practice Repository

This repository contains artifacts for manual testing practice:

* **testcases.txt** → Core test cases  
* **testcases2.txt** → Bug validation scenarios  
* **queries.sql** → SQL queries for DB validation  
* **testplan.md** → Test plan documentation  
* **Postman/postman/collections/** → API test collections  

Bugs are tracked via GitHub Issues and linked to commits.

## 🧪 API Testing with Postman

This repository includes Postman collections used for API validation and practice. The setup was initialized using Postman's local Git integration, which created two folders:

- `.postman/` — contains internal Postman configuration files (e.g., workspace settings, globals)  
- `postman/` — contains actual API collections used for testing  

### 📁 Collection Files

All API test collections are stored in:
Postman/postman/collections/

Included files:
- `my_collection.json` → API endpoints for practice and validation  
- `practice_collection.json` → Additional scenarios for exploring request/response behavior  

### 🔗 How They Fit Into QA Workflow

- **Manual Testing** → Validates user-facing flows (login, signup, etc.)  
- **SQL Scripts** → Confirms backend data integrity  
- **Postman Collections** → Exercises APIs directly, even for scenarios not covered in manual test cases  
- **Bug Reports** → Capture discrepancies across UI, API, and database layers  

This layered approach ensures broader QA coverage by testing both user-facing and backend components.

---

## 📂 Repository Structure

Included files:
- `my_collection.json` → API endpoints for practice and validation  
- `practice_collection.json` → Additional scenarios for exploring request/response behavior  

### 🔗 How They Fit Into QA Workflow

- **Manual Testing** → Validates user-facing flows (login, signup, etc.)  
- **SQL Scripts** → Confirms backend data integrity  
- **Postman Collections** → Exercises APIs directly, even for scenarios not covered in manual test cases  
- **Bug Reports** → Capture discrepancies across UI, API, and database layers  

This layered approach ensures broader QA coverage by testing both user-facing and backend components.

---

## 📂 Repository Structure


qa-practice/ ├── Postman/ │   ├── .postman/                # Internal Postman config (workspace, globals) │   └── postman/ │       └── collections/ │           ├── my_collection.json │           └── practice_collection.json ├── README.md ├── testcases.txt ├── testcases2.txt ├── queries.sql └── testplan.md


