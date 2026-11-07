# RAPIDD Technologies – C# Assignment  
**Candidate:** Varun S

**Date:** October 2026 

---

## 📋 Objective  
This project was created as part of the RAPIDD Technologies hiring process.  
It retrieves employee time entries from the given API endpoint, calculates the total hours worked for each employee, and visualizes the results using both an **HTML table** and a **Pie Chart (PNG image)**.

---

## 🧰 Tools & Technologies  
- **Language:** C#  
- **Framework:** .NET 8 (compatible with .NET 6)  
- **IDE:** Visual Studio 2022  
- **Libraries Used:**
  - `System.Net.Http` → Fetch data from REST API  
  - `System.Text.Json` → Deserialize JSON  
  - `System.Drawing.Common` → Generate Pie Chart (PNG image)  

---

## ⚙️ How It Works  

1. **Fetch Data:**  
   The program calls the RAPIDD API endpoint:
  ' https://rc-vault-fap-live-1.azurewebsites.net/api/gettimeentries?code=vO17RnE8vuzXzPJo5eaLLjXjmRW07law99QTD90zat9FfOQJKKUcgQ== '


3. **Calculate Hours:**  
It calculates the total number of hours worked per employee by subtracting `StarTimeUtc` from `EndTimeUtc`.

4. **Generate HTML Report:**  
- Displays each employee’s name and total hours.  
- Highlights rows in **red** if the employee worked less than 100 hours.

4. **Generate Pie Chart:**  
- Creates `EmployeePieChart.png` showing the percentage of total hours worked per employee.

---

## 🧱 Project Structure  

RAPIDD_Assignment/
│
├── Program.cs # Main C# code
├── EmployeeReport.html # Generated HTML table
├── EmployeePieChart.png # Generated pie chart
├── Varun s_C# Assignment.exe # Final executable file
└── README.md # Project documentation


---

## 🧩 How to Run  

### ▶️ Run via Visual Studio 2022
1. Open `RAPIDD_Assignment.sln` or `Program.cs` in **Visual Studio 2022**  
2. Press **Ctrl + F5** (Run Without Debugging)  
3. The program will:
   - Fetch data from API  
   - Generate `EmployeeReport.html`  
   - Generate `EmployeePieChart.png`

### ⚙️ Build Executable (.exe)
1. In Visual Studio, right-click your project → **Publish**  
2. Choose **Folder**  
3. Under **File Options**, check ✅ **Produce single file**  
4. Set Target Runtime → `win-x64`  
5. Click **Publish**  

The `.exe` will be created in:  

Varun S_C# Assignment.exe
---

## 📊 Output Files  

| File | Description |
|------|--------------|
| **EmployeeReport.html** | Table showing total hours worked by each employee |
| **EmployeePieChart.png** | Pie chart showing percentage of total time worked |
| **ManasNath_C# Assignment.exe** | Executable file for submission |

---

## 📤 Submission Information  
- GitHub Repository: https://github.com/varun782/Rappido.git
- Executable File: Uploaded to RAPIDD hiring portal  
- Confirmation Email: Sent to HR  

---

## 🧠 Notes  
- The project automatically handles null or empty employee names.  
- Rows with less than 100 hours are highlighted in red.  
- Compatible with both `.NET 6` and `.NET 8`.

---

© 2026 — **Varun S**
 


