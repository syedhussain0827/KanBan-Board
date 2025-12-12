📌 Kanban Task Management App

A simple and interactive Kanban Board built using HTML, CSS, and Vanilla JavaScript.
This project allows users to create tasks, drag & drop them across different stages, and automatically saves all tasks in localStorage so nothing is lost on refresh.

🚀 Features

✅ Add New Tasks
Click “Add New Task” to open a modal.
Enter Task Title and Task Description.

🎯 Drag & Drop Support
Move tasks between To Do, In Progress, and Done columns.
Smooth UI effects while dragging & dropping.

💾 Auto Save (localStorage)
Tasks remain saved even after refreshing the browser.
Saved by column (todo, progress, done).

🗑 Delete Tasks
Each task has a delete button.

🎨 Responsive & Clean UI
Dark theme
Modern animations
Mobile-friendly layout

📘 How It Works
1️⃣ Add Task

User fills the form → Clicks Add Task → Task is added to To Do column.

2️⃣ Drag & Drop
Move tasks freely between columns:

column.addEventListener("drop", () => {
    column.appendChild(dragElement);
    upadateTaskCounts();
});

3️⃣ Local Storage
Every update saves tasks:
localStorage.setItem("tasks", JSON.stringify(tasksData));

4️⃣ Load Saved Tasks
When the page loads, tasks are restored automatically.
