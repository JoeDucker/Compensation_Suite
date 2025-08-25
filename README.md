# Employee Compensation Forecasting & Analysis App

An integrated desktop application that enables HR and business teams to analyze, forecast, and manage employee compensation. Built with **Visual Basic, C# (WinForms), SQL Server, and Power BI**, the app combines structured data storage, interactive UI, and rich visual dashboards.

---

## ✨ Features

* 📋 **Data View**

  * View all employees with their role, location, and compensation.
  * Search by employee name or ID.
  * Filter by role and location.

* 📊 **Analytics & Dashboards**

  * Bar chart: Average compensation by role.
  * Pie chart: Compensation distribution by location.
  * Line chart: Compensation trends over time.
  * Interactive filters that dynamically update visualizations.

* 🖊️ **Compensation Updates**

  * Update employee compensation directly from the application.
  * Maintain an **audit trail** for transparency (who changed, what changed, when, why).

* 📤 **Data Export**

  * Export employee records into CSV format for offline reporting.

* 🔐 **Audit Trail**

  * Full history of compensation updates, with change reason and system metadata.

---

## 🛠️ Tech Stack

* **Frontend:** C# (Windows Forms), Visual Basic (UI & integration)
* **Backend:** SQL Server (tables, stored procedures, audit log)
* **BI Visualization:** Power BI
* **Languages:** C#, Visual Basic, SQL

---

## 📂 Project Structure

```
├── EmployeeCompensationApp/       # Visual Studio WinForms solution
│   ├── MainForm.cs                # Main UI logic (C#)
│   ├── EditCompensationDialog.cs  # Edit dialog for updating compensation
│   └── ...
├── SQL/                           # Database schema & stored procedures
│   ├── schema.sql                 # Tables (Employee, Role, Location, Assignment, Audit)
│   └── usp_UpdateCompensationWithAudit.sql
├── PowerBI/                       # Power BI .pbix dashboards
├── README.md
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/employee-compensation-app.git
```

### 2. Database Setup

* Open SQL Server Management Studio (SSMS).
* Run the scripts in the `/SQL` folder to create tables and stored procedures.
* Ensure the database name matches the connection string.

### 3. Configure Connection String

* In `App.config`, update the connection string:

```xml
<connectionStrings>
  <add name="EmployeeDb"
       connectionString="Server=YOUR_SERVER;Database=employee;Trusted_Connection=True;TrustServerCertificate=True;"
       providerName="System.Data.SqlClient" />
</connectionStrings>
```

### 4. Run the App

* Open the solution in Visual Studio.
* Build and run the project.

---

## 📈 Power BI Dashboards

Power BI is used to provide additional analytical capabilities. Import the `Application_demo.pbix` file to explore interactive dashboards.

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
