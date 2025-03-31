# 📚 Student Learning Activity Analysis  

## 📌 Overview  
This project analyzes student learning activities, performance, and engagement using **SQL**.  
The dataset includes student details such as names, enrollment date, contact numbers, co-curricular activities, scores, and attendance.  

## 🗂️ Dataset Description  
The dataset captures detailed information about students' learning behaviors:  

| Column Name               | Description                                       | Example          |
|---------------------------|---------------------------------------------------|------------------|
| **first_name**            | First name of the student                        | "Sandeep"        |
| **last_name**             | Last name of the student                         | "Sinha"          |
| **contact_number**        | Student’s contact number                         | "9012363880"     |
| **enrolled_date**         | Date when the student enrolled                   | "6/20/2023"      |
| **hours_spend**           | Hours spent on co-curricular activities          | "27"             |
| **score**                 | Score obtained by the student                    | "127"            |
| **co_curricular_activity**| The activity the student is involved in          | "Dance"          |
| **attendance%**           | Student’s attendance percentage                  | "90-100"         |

## 🏗️ Steps Performed  
1. **Data Retrieval:** Extracting student data using SQL queries.  
2. **Data Cleaning:** Formatting names, removing extra spaces, and processing values.  
3. **Data Analysis:** Extracting insights about student performance and activities.  

## 🛠️ Technologies Used  
- **SQL** 🏆 - Data querying and analysis  
- **SQLite** 🗄️ - Database storage for student records  
- **Python (Optional)** 🐍 - Used for database setup and loading data  

## 🏗️ SQL Tasks Performed  
### ✅ Task 1: Retrieve Student Data  
Retrieve all available student records from the `stdata` table.  

### ✅ Task 2: Retrieve Contact Number & Length  
- Extract **contact number** and **calculate its length**.  

### ✅ Task 3: Retrieve Contact Numbers of Length 9  
- Extract contact numbers where the length is exactly **9**.  
- Name the length column as `len`.  

### ✅ Task 4: Process Co-Curricular Activity Data  
- Retrieve **First Name, Last Name, Co-Curricular Activity (`cca`)**.  
- Calculate its **length (`len_cca`)**.  
- **Trim** extra spaces (`trim_cca`).  
- Calculate the length of the **trimmed** column (`len_trim_cca`).  

### ✅ Task 5: Retrieve First & Last Name in Lowercase  
Convert both **First Name** and **Last Name** to lowercase.  

### ✅ Task 6: Retrieve First & Last Name in Uppercase  
Convert both names to **uppercase**.  

### ✅ Task 7: Create Full Name in Lowercase  
- Convert both names to **lowercase**.  
- Concatenate them with a **space** in between.  
- Name this column `full_name`.  

### ✅ Task 8: Generate Student Email ID  
- Convert names to **lowercase**.  
- Remove extra spaces.  
- Format: `firstname.lastname@apscollege.org`.  
- Name this column `emailid`.  

### ✅ Task 9: Extract First Letter & Capitalize Name  
- Extract the **first letter** of the first name (`first_letter`).  
- Convert the first letter to **uppercase** (`upper_first_letter`).  
- Convert full name to **Proper Case** (`proper_name`).  

### ✅ Task 10: Generate Student Initials  
- Extract **first letter** of First and Last Name.  
- Concatenate them to form **initials** (e.g., "SS").  

### ✅ Task 11: Format Full Name & Extract Enrollment Year  
- Convert **First & Last Name** to **Proper Case** (`proper_full_name`).  
- Extract **Enrollment Year** using `SUBSTR()`.  

### ✅ Task 12: Generate & Format Email ID  
- Convert names to **lowercase**.  
- Format: `firstname.lastname@apscollege.org`.  
- Replace **double dots** (`..`) with **single dot** (`.`).  
- Name the column `finalemailid`.  

### ✅ Task 13: Count Total Email IDs  
Count the total number of email IDs.  

### ✅ Task 14: Count Unique Email IDs  
Count the **unique** email IDs.  

### ✅ Task 15: Retrieve Students with Last Name Starting with 'S'  
- Extract **First Name, Last Name, and Score**.  
- Filter records where **Last Name starts with 'S'**.  

### ✅ Task 16: Retrieve Students with Single-Letter Last Name  
- List students with a **single-letter Last Name**.  
- Exclude cases where **Last Name is a full stop (.)**.  

### ✅ Task 17: Co-Curricular Activity Analysis (2024)  
- Retrieve **Total Score & Participants** for each activity.  
- Extract **Enrollment Year** using `SUBSTR()`.  
- **Sort** results by `total_score` in **descending order**.  
- Output Columns: `co_curricular_activity, enrolled_year, total_score, participant_count`.  