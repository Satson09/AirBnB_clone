# **0x00. AirBnB Clone - The Console**

## **Project Overview**
- **Type:** Group Project (2 members)
- **Topic:** Python OOP
- **Instructor:** Guillaume
- **Weight:** 5
- **Team Members:** Satson Johnson
- **Status:** Ongoing Second Chance Project
- **Start Date:** October 9, 2023, 6:00 AM
- **Deadline:** October 18, 2023, 6:00 AM
- **Reviews:**
  - **Manual QA Review:** Must be requested upon project completion
  - **Auto QA Review:** Will be launched at the deadline
  - **Current Review Status:**
    - Contribution: **100.0%**
    - Manual QA Review: **In second deadline**
    - Auto QA Review: **0.0/302 (mandatory)** & **0.0/233 (optional)**
    - Overall: **Waiting on some reviews**

## **Concepts to Explore**
For this project, you are expected to study the following concepts:
- Python Packages
- AirBnB Clone

---

## **Background Context**
### **Welcome to the AirBnB Clone Project!**
Before starting, read the **AirBnB Concept Page**.

#### **First Step: Building a Command Interpreter**
This is the initial step toward developing your first full web application: the **AirBnB Clone**. This phase is crucial because it sets the foundation for subsequent projects, including:
- HTML/CSS templating
- Database storage
- API integration
- Front-end development

Each task in this project contributes to:
- Creating a **parent class (BaseModel)** to handle:
  - Initialization
  - Serialization & Deserialization of future instances
- Establishing a serialization/deserialization flow:
  - **Instance ↔ Dictionary ↔ JSON String ↔ File**
- Developing all necessary AirBnB classes:
  - `User`, `State`, `City`, `Place`, etc. (inheriting from BaseModel)
- Implementing the **first abstracted storage engine**: **File Storage**
- Writing **unit tests** to validate all classes and the storage engine

### **What is a Command Interpreter?**
It functions similarly to a Shell but is limited to a specific use case: **managing project objects**.

With this interpreter, you can:
- **Create** new objects (e.g., User, Place)
- **Retrieve** objects from a file/database
- **Perform operations** (e.g., count objects, compute statistics)
- **Update attributes** of an object
- **Destroy** an object

---

## **Resources**
Read or watch:
- [cmd module](https://docs.python.org/3/library/cmd.html)
- [cmd module in depth](https://pymotw.com/3/cmd/)
- [Python Packages Concept](https://docs.python.org/3/tutorial/modules.html)
- [UUID Module](https://docs.python.org/3/library/uuid.html)
- [datetime Module](https://docs.python.org/3/library/datetime.html)
- [unittest Module](https://docs.python.org/3/library/unittest.html)
- [args & kwargs](https://realpython.com/python-kwargs-and-args/)
- [Python Test Cheatsheet](https://docs.python.org/3/library/unittest.html)
- [cmd Module Wiki](https://en.wikipedia.org/wiki/Cmd)
- [Python Unittest Guide](https://realpython.com/python-testing/)

---

## **Learning Objectives**
By the end of this project, you should be able to explain:

### **General Concepts:**
- How to create a **Python package**
- How to create a **command interpreter** using the `cmd` module
- What **unit testing** is and how to implement it in large projects
- How to **serialize and deserialize a class**
- How to **write and read a JSON file**
- How to **manage datetime** objects in Python
- What a **UUID** is and how it works
- How to use **args** (`*args`) and **kwargs** (`**kwargs`)
- How to handle **named arguments** in a function

---

## **Project Execution Process**

### **1. Environment Setup**
- Ensure you have **Python 3.8.5** installed.
- Install required dependencies using:
  ```bash
  pip install -r requirements.txt
  ```
- Clone the repository:
  ```bash
  git clone [https://github.com/Satson09/AirBnB_clone.git]
  cd AirBnB_clone
  ```

### **2. Running the Command Interpreter**
- Launch the console:
  ```bash
  ./console.py
  ```
- Sample Commands:
  ```bash
  (hbnb) create User
  (hbnb) show User 1234-5678-9012
  (hbnb) all User
  (hbnb) update User 1234-5678-9012 email "example@mail.com"
  (hbnb) destroy User 1234-5678-9012
  (hbnb) quit
  ```

### **3. Code Structure**
- **`models/base_model.py`**: Defines `BaseModel` class.
- **`models/user.py`**: Defines `User` class.
- **`models/state.py`**: Defines `State` class.
- **`models/city.py`**: Defines `City` class.
- **`models/place.py`**: Defines `Place` class.
- **`models/engine/file_storage.py`**: Handles object storage.
- **`console.py`**: Entry point for the command interpreter.

### **4. Testing the Project**
- Run unit tests:
  ```bash
  python3 -m unittest discover tests
  ```

### **5. Expected Output Example**
```bash
(hbnb) create User
56d43177-cc5f-4d6c-a0c1-e167f8c27337
(hbnb) show User 56d43177-cc5f-4d6c-a0c1-e167f8c27337
[User] (56d43177-cc5f-4d6c-a0c1-e167f8c27337) {'id': '56d43177-cc5f-4d6c-a0c1-e167f8c27337', 'created_at': '2023-10-09T06:00:00.000000', 'updated_at': '2023-10-09T06:00:00.000000'}
(hbnb) quit
```

---

## **Project Guidelines**
### **Requirements**
- All files must be **PEP8 compliant** (`pycodestyle` version 2.8).
- Use **vi, vim, or emacs** as editors.
- All files must end with a **new line**.
- Code should be documented using **docstrings**.

### **Plagiarism Warning**
- Do **not** copy code from others.
- Publishing any content from this project is **strictly forbidden**.
- Plagiarism will result in **removal from the program**.

---

## **Conclusion**
This project is the foundation of the **AirBnB Clone** and serves as the base for future development. Follow best practices, write clean code, and adhere to the project requirements to succeed.

Happy Coding!

