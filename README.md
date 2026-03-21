# 🧠 Supreme JMS | Job Management System

The workflow engine for **Supreme Outdoor Advertising Ltd.** This system manages the lifecycle of advertising projects from initial intake to final installation.

## 🏗️ System Architecture
This app provides the **Production Intelligence** for the [Supreme HQ Hub](LINK_TO_YOUR_HQ_REPO).
- **Backend**: Google Sheets (Workflow Database) + Apps Script (API).
- **Frontend**: GitHub Pages (Operator Dashboard).

---

## 🚀 Key Functionalities
- **Print Queue Management**: Filtered views for **Yotta H3200KJ** and **Meitu** operators to see only relevant active jobs.
- **Artwork Approval Tracker**: Status-based color coding (Pending, Approved, Printing, Completed).
- **Carnival 2026 Production**: Specialized priority flags for seasonal high-volume projects.
- **Capacity Fetching**: Provides real-time "Active Job" and "Queue Count" stats to the Master Hub.

---

## 🔧 Google Apps Script Integration
The `Code.gs` file in the JMS Google Sheet handles the following API actions:
- `GET_COUNT`: Returns the total number of non-completed jobs for the HQ dashboard.
- `GET_QUEUE`: Fetches a list of all jobs currently marked as "Ready for Print."
- `UPDATE_STATUS`: Allows operators to move a job from "Printing" to "Finished" directly from the floor.

---

## 🚦 Production Workflow
1. **Intake**: Sales/Design enters job details into the Master Google Sheet.
2. **Approval**: Artwork is verified and marked "Approved."
3. **Queue**: Job automatically appears in the JMS Frontend for the assigned printer.
4. **Completion**: Operator marks job as "Done," triggering an update to the Inventory Sheet for material deduction.

---

## 📝 Change Log
- **March 21**: Optimized `GET_QUEUE` logic to support faster loading on mobile devices.
- **March 10**: Implemented machine-specific filtering (UV vs. Solvent).
- **February 28**: Integrated "Joint Tribute" script logic for family estate events.

---

## 👤 Administrator
**Damian A. Moncrieffe**# supreme-jms

