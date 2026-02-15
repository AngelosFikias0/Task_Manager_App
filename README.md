# Task Manager

> **A focused productivity tool for managing workflows through dynamic task tracking, real-time status updates, and automated list organization.**

This application is a study in **event-driven architecture** and **State-to-UI synchronization**. It provides a frictionless experience for organizing daily goals while ensuring data integrity through automated task validation.

---

## 📌 System Workflow

The application manages two distinct states: **Current** and **Completed**. The logic ensures a smooth transition between these states while updating global counters.



```text
       [ User Input ]
       (Task Description)
              |
      [ Validation Engine ]
      (Check for Uniqueness)
              |
      /-------+-------\
      |               |
 [ Valid ]       [ Duplicate ]
      |               |
      v               v
 [ Add to List ]   [ Alert User ]
      |
      +-----> [ Update Counters ]
      |
      v
 [ Move to Completed ]
 (On User Click)
```

---

## 🚀 Key Features

* **Smart Task Creation:** Seamlessly add new entries to the "Current" queue.
* **State Transition Logic:** One-click functionality to migrate tasks from active status to "Completed."
* **Real-Time Analytics:** Dynamic counters that provide an immediate visual summary of workload and accomplishments.

* **Collision Prevention:** Integrated logic that enforces **Unique Task Names**, preventing redundant entries and maintaining a clean workspace.
* **Responsive Task View:** A mobile-friendly layout that ensures your to-do list is accessible across all devices.

---

## 🧰 Technical Stack

| Category | Technology |
| :--- | :--- |
| **Structure** | HTML5 (Semantic Task Lists) |
| **Styling** | CSS3 (Transitions & Responsive Layouts) |
| **Logic** | Vanilla JavaScript (ES6+) |
| **Persistence** | DOM-based state management |

---

## 📊 Logic & Performance

* **DOM Manipulation:** Optimized to handle dynamic creation and removal of elements without full page reloads.
* **Array Management:** Uses JavaScript arrays to track task metadata, ensuring high-speed validation for unique names.
* **Event Delegation:** Efficiently manages clicks across multiple list items, reducing memory overhead.

---

## 🛠️ Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/AngelosFikias0/Task_Manager.git](https://github.com/AngelosFikias0/Task_Manager.git)
   cd Task_Manager
   ```
2. **Launch:**
   Open `index.html` in your browser to start organizing your day.

---

## 📈 Engineering Highlights

* **UX Feedback:** Implemented visual cues (like strikethroughs or color shifts) to signify completed actions.
* **Data Integrity:** The uniqueness check prevents common user errors and ensures a "source of truth" for every task.
* **Code Modularity:** Functions are separated into creation, transition, and counting logic for easy maintenance.

---

## 📄 License
This project is licensed under the **MIT License**.

---
**Developed by Angelos Fikias** *Optimizing personal productivity through clean code and efficient logic.*
