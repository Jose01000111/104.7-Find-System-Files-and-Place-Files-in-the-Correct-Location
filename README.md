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

bash
Copy
Edit
ls /  

### 🔹 Explore Purpose of Each Directory

bash
Copy
Edit
man hier  

### 🔹 Verify Standard Directories Exist

Check for /etc, /bin, /usr, /var, /tmp, /home, /opt.

## 2️⃣ Finding Files with find

### 🔹 Find All Files Named passwd

bash
Copy
Edit
sudo find / -name passwd  

### 🔹 Find All Files in /etc Modified in Last 2 Days

bash
Copy
Edit
sudo find /etc -mtime -2  

### 🔹 Find Executables Larger than 10MB

bash
Copy
Edit
sudo find / -type f -executable -size +10M  

## 3️⃣ Using locate and updatedb

### 🔹 Update the File Database

bash
Copy
Edit
sudo updatedb  

### 🔹 Locate Bash Binary

bash
Copy
Edit
locate bin/bash  

### 🔹 Review the updatedb Configuration

bash
Copy
Edit
cat /etc/updatedb.conf  

## 4️⃣ Using whereis, which, and type

### 🔹 Locate the Path of the ls Command

bash
Copy
Edit
whereis ls  

### 🔹 Display Path for grep

bash
Copy
Edit
which grep  

### 🔹 Determine Type of Command (alias, builtin, file)

bash
Copy
Edit
type cd  
type ls  

## 📘 What I Learned
In this lab, I learned how to identify the location of important files and directories using several Linux utilities 🔍. I became familiar with the Filesystem Hierarchy Standard and the expected placement of different types of files. I also learned how to update and use the file search index with updatedb and locate. This knowledge is essential for troubleshooting, system maintenance, and understanding how Linux systems are organized 
