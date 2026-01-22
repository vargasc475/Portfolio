# 📝 Persistent To-Do List (Vanilla JS)
A clean, minimalist To-Do List application built with Vanilla JavaScript. This project focuses on Data Persistence, ensuring that your tasks remain available even after closing the browser or refreshing the page.

## 🚀 Features
- Add Tasks: Quickly jot down new items.
- Mark as Complete: Toggle tasks as "done" with a single click.
- Delete Tasks: Remove individual items or clear the entire list.
- Data Persistence: Integrated with the Web Storage API (localStorage).
- Responsive Design: Fully functional on desktop, tablet, and mobile devices.

## 🛠️ Technology Stack
- HTML5: Semantic structure for the task interface.
- CSS3: Custom styling with Flexbox/Grid for a modern look.
- JavaScript (ES6+): DOM manipulation, event handling, and logic.
- LocalStorage: Client-side storage to save task arrays as JSON strings.

## 💾 How LocalStorage is Used
This project implements the browser's localStorage to prevent data loss. The logic follows this workflow:

1. Saving Data: Whenever a task is added or modified, the current array of objects is converted to a string using JSON.stringify() and saved under a specific key.
2. Retrieving Data: On page load, the app checks for the key using localStorage.getItem().
3. Parsing: If data exists, it is converted back into a JavaScript object using JSON.parse() and rendered to the DOM.

## 🔗 Live Demo

Experience the live application here:  
👉 **[Launch To-Do List App](https://vargasc475.github.io/Portfolio/ToDoList)**

---

⚙️ Installation & Setup
Since this is a client-side project, no server-side setup is required.

1. Clone the repository:

Bash
git clone https://github.com/yourusername/todo-list-js.git

2. Navigate to the project folder:

Bash
cd todo-list-js

3. Open the app: Simply open index.html in your favorite web browser.

## 🖥️ Usage
1. Type your task in the input field.
2. Press Enter or click the "Add" button.
3. Click on a task's text to mark it as completed (it will be crossed out).
4. Click the "Delete" (X) button to remove a specific task.
5. Refresh the page—notice your tasks are still there!

## 🔮 Future Improvements
- [ ] Add categories/tags (Work, Personal, Urgent).
- [ ] Implement a "Dark Mode" toggle.
- [ ] Add drag-and-drop reordering.
- [ ] Include a "Clear All Completed" button.
