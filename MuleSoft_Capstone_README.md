# MuleSoft DataWeave Capstone Project -- Student Enrollment Transformation

## 📌 Project Overview

This capstone project focuses on transforming student enrollment data
from **JSON**, **XML**, and **CSV** into a **standardized JSON API
response** using DataWeave.

## 🎯 Objective

Transform and process student enrollment data coming from different
formats and convert it into a standardized API response.

## 🧩 Scenario

A university receives student enrollment data from multiple departments
in different formats.\
Your task is to convert all incoming data into one **standard JSON
structure**.

## 📥 Input Formats

The project includes: - JSON input - XML input - CSV input

## 📤 Required Output Format

``` json
{
  "university": "Global Tech University",
  "students": [
    {
      "studentId": "",
      "fullName": "",
      "age": "",
      "department": "",
      "status": "ACTIVE"
    }
  ]
}
```

## ✅ Tasks

### Task 1 -- JSON Transformation

-   Map `id → studentId`
-   Map `name → fullName`
-   Keep `age`
-   Keep `department`
-   Add `"status": "ACTIVE"`

### Task 2 -- XML to JSON Transformation

Convert XML input to required JSON structure.

### Task 3 -- CSV to JSON Transformation

Transform CSV input into standard JSON format.

### Task 4 -- Filtering

Only include students with:

    age >= 22

### Task 5 -- Sorting

Sort students by **name alphabetically**.

## ⭐ Bonus Tasks

### 1. Add Category Field

-   `"Junior"` if age \< 23
-   `"Senior"` if age \>= 23

### 2. Count Students

Add:

``` json
"totalStudents": number
```

### 3. Uppercase Names

Convert all names to uppercase.

## 🏗 Suggested Project Structure

    mulesoft-capstone/
    │
    ├── src/main/mule/
    │   └── student-enrollment.xml
    │
    ├── src/main/resources/
    │   ├── students.json
    │   ├── students.xml
    │   └── students.csv
    │
    └── README.md

## 🚀 Expected Features

-   Multi-format input processing
-   DataWeave transformations
-   Filtering
-   Sorting
-   Conditional logic
-   Aggregation
-   Standard API response

## 🧪 Example Output

``` json
{
  "university": "Global Tech University",
  "totalStudents": 3,
  "students": [
    {
      "studentId": "101",
      "fullName": "ABEL TESFAYE",
      "age": 22,
      "department": "Computer Science",
      "status": "ACTIVE",
      "category": "Junior"
    }
  ]
}
```

## 🎓 Learning Outcomes

By completing this project students will learn: - DataWeave
transformations - JSON, XML, CSV parsing - Filtering & sorting -
Conditional mapping - Aggregation - API response standardization

## 🛠 Technology

-   MuleSoft 4
-   DataWeave 2.0
-   Anypoint Studio

## 👨‍💻 Author

Capstone Project -- Craft Knowledge MuleSoft Training
