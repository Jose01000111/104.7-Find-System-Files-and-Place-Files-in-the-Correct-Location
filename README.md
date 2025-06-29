# 📁104.7: Find System Files and Place Files in the Correct Location

## ✅ What I Did in This Lab
I used various file location commands to search for binaries, scripts, and configuration files on the system. I explored the structure of the Linux filesystem and confirmed if files are located where they’re supposed to be according to the FHS 📘. I also configured the updatedb service to update the file search index.

I’ve included some helpful links to guide you through the lab and for studying afterward:

[EXAM OBJECTIVE 104.7](https://www.lpi.org/our-certifications/exam-101-102-objectives/#104.7_Find_system_files_and_place_files_in_the_correct_location)

[OBJ. 104.7 NOTES](https://1drv.ms/w/c/354f1c8d534fbced/ESsAHgPWeqBFlBD-vYbNmiQBaEO2Yl6IWQaaD0pSNOMJDg?e=b9lEgE)

[OBJ. 104.7 LAB](https://1drv.ms/w/c/354f1c8d534fbced/EXdWdFCSZptBtAEnCH4sOX4Bp03EHHaA3BBk26rwSBOxog?e=DPRckH)

---

## 1️⃣ Understanding the FHS File Locations 

### 🔹 List Top-Level Directories

 ![CAvh4jw](https://github.com/user-attachments/assets/08db935f-bc96-4292-b843-39c11bf505e7)

### 🔹 Explore Purpose of Each Directory

![XoHl4Um](https://github.com/user-attachments/assets/63d8af8a-d731-409c-a735-98d25227ef62)

### 🔹 Verify Standard Directories Exist

![NeIW00w](https://github.com/user-attachments/assets/ee959476-d282-411a-afd4-1036ca82b632)

## 2️⃣ Finding Files with find

### 🔹 Find All Files Named passwd

![6KTL55S](https://github.com/user-attachments/assets/6ca645ef-9b9a-412a-82fb-796c80864cd0)

### 🔹 Find All Files in /etc Modified in Last 2 Days

![2jfzJas](https://github.com/user-attachments/assets/a6f27556-aa16-4542-856f-9434ffc13a19)

### 🔹 Find Executables Larger than 10MB

![oRw61XO](https://github.com/user-attachments/assets/77a6d020-605d-4ebc-bc01-536d01c2d404)

## 3️⃣ Using locate and updatedb

### 🔹 Update the File Database

### 🔹 Locate Bash Binary

![2RCytma](https://github.com/user-attachments/assets/ef18108c-003f-4e6c-968b-1453bf7975f2)

### 🔹 Review the updatedb Configuration

![FBEXsYH](https://github.com/user-attachments/assets/ec49ba6d-3521-4097-ae28-24b680c24e75)

## 4️⃣ Using whereis, which, and type

### 🔹 Locate the Path of the ls Command

### 🔹 Display Path for grep

### 🔹 Determine Type of Command (alias, builtin, file)

![xYe6ozi](https://github.com/user-attachments/assets/9e67393d-9c0f-4e5a-a526-7932b55d2bc4)

---

## 📘 What I Learned
In this lab, I learned how to identify the location of important files and directories using several Linux utilities 🔍. I became familiar with the Filesystem Hierarchy Standard and the expected placement of different types of files. I also learned how to update and use the file search index with updatedb and locate. This knowledge is essential for troubleshooting, system maintenance, and understanding how Linux systems are organized 
