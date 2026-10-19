# 💬 Live Chat Application — Setup Guide

## 📌 Introduction

This guide explains how to set up and run the Live Chat Application developed using HTML5, CSS3, and JavaScript.

The application uses the BroadcastChannel API to communicate between browser tabs without requiring a backend server or database.

---

## 🛠️ Prerequisites

Before running the application, make sure you have:

- A modern web browser (Google Chrome, Microsoft Edge, or Firefox).
- Visual Studio Code (optional).
- Git (optional, for cloning the repository).

No Node.js, npm, or database installation is required.

---

## 🚀 Installation

### Step 1: Clone the Repository

Open your terminal and run:

```bash
git clone https://github.com/sagarmeena004/Chat-App.git
```

**Note:** Replace the repository URL if your GitHub repository has a different name.

### Step 2: Open the Project Folder

Navigate to the downloaded project folder.

```bash
cd Chat-App
```

### Step 3: Verify Project Files

Ensure the following files are present:

```text
chatapp msme/
│
├── index.html
├── dark-theme-background-q62o6998n8bqxzrf.jpg.jpeg
├── README.md
├── FEATURES.md
├── SETUP.md
├── TECHNOLOGIES.md
├── CHANGELOG.md
└── .gitignore
```

### Step 4: Run the Application

Open `index.html` in a modern web browser.

For more consistent testing, you can also use a local development server such as VS Code Live Server.

No backend configuration is required.

---

## 💬 How to Use

1. Open the Chat Application in your browser.
2. Open the same application URL in another browser tab.
3. Enter a message in the text input field.
4. Click the **Send** button or press **Enter**.
5. The message will appear in the connected browser tab.
6. Continue sending messages between the tabs.

---

## 🔄 How Cross-Tab Communication Works

The application uses the JavaScript BroadcastChannel API.

```javascript
const channel = new BroadcastChannel('live_chat_frontend');
```

When a message is sent, the application broadcasts it to other connected tabs.

The receiving tabs listen for incoming messages and update their chat interface.

Communication works between compatible browsing contexts sharing the same origin and storage partition.

---

## 🧪 Testing

### Test 1: Send a Message

- Open the application in two tabs.
- Type a message in the first tab.
- Click Send.
- Verify that the message appears in the second tab.

### Test 2: Enter Key

- Type a message.
- Press Enter.
- Verify that the message is sent.

### Test 3: Multiple Tabs

- Open the application in three browser tabs.
- Send a message from one tab.
- Verify that the other connected tabs receive it.

### Test 4: Tab Notifications

- Open a new tab containing the application.
- Check the connected tab notifications.
- Close a tab and observe the leave notification.

---

## ⚠️ Important Notes

- This application is designed for communication between browser tabs, not different devices over the internet.
- Messages are not saved permanently.
- Refreshing the page clears the displayed chat history.
- No user login or authentication is required.
- No backend server or database is used.

---

## 👨‍💻 Developer

**GitHub:** sagarmeena004

**Project:** Live Chat Application

**Technologies:** HTML5, CSS3, JavaScript