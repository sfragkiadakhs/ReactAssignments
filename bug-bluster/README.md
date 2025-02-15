# 🚀 Getting Started with **Bug Bluster**

This application is designed to help understand the use of **Reducers in React** through a simple **ticketing system**.

## 🎯 Application Overview

The UI consists of the following elements:

- A **form** with fields for **title, description, and priority**, allowing users to create or edit tickets.
- A **list of created tickets**, sorted **by default from high to low priority**.
  - Available priority levels: **low, medium, high**.

Since tickets have different states, we use a **ticket reducer** to manage them efficiently.

---

## 🔧 State Management with Reducers

The application includes the following **states and actions**:

1. **Tickets State**

   - Actions: `ADD_TICKET`, `UPDATE_TICKET`, `DELETE_TICKET`

2. **Editing Ticket State**

   - Tracks whether a ticket is being edited.
   - Actions: `SET_EDITING_TICKET`, `CLEAR_EDITING_TICKET`

3. **Sorting State**
   - Stores the selected sorting method for tickets.
   - Action: `SET_SORTING`

---

## 🛠 Available Scripts

Run the following command in the project directory:

### **Start the development server**

```sh
npm start
```

Runs the app in development mode.  
Open [http://localhost:3000](http://localhost:3000) in your browser to view it.

---
