# 💬 Live Chat Application — Features

## 📌 Overview

Live Chat Application is a frontend-based messaging project developed using HTML5, CSS3, and JavaScript.

It uses the BroadcastChannel API to enable real-time communication between multiple browser tabs of the same origin.

The application does not require a backend server, database, or external JavaScript framework.

---

## 🚀 Core Features

### 1. Real-Time Cross-Tab Messaging

- Send and receive messages between browser tabs.
- Messages appear instantly in connected tabs.
- Communication is handled using the BroadcastChannel API.
- No page refresh is required.

### 2. Modern Chat Interface

- Clean and user-friendly design.
- WhatsApp-inspired message bubbles.
- Separate styling for sent and received messages.
- Smooth message appearance animation.

### 3. Dark-Themed Background

- Custom background image for the chat area.
- Modern visual appearance.
- Comfortable and attractive chat interface.

### 4. Active Tab Detection

- Detects communication from other browser tabs.
- Displays the number of known connected tabs.
- Uses heartbeat messages to identify active tabs.
- Displays notifications when tabs join or leave.

**Note:** The current implementation does not automatically remove every inactive tab after a missed heartbeat.

### 5. Message Timestamps

- Displays the time associated with each message.
- Helps users identify when messages were sent.

### 6. Send Messages Using Enter

- Users can send messages by clicking the Send button.
- Pressing Enter also sends the message.
- Empty messages are ignored.

### 7. Automatic Chat Scrolling

- Automatically scrolls to the latest message.
- Keeps recent conversations visible.

### 8. Responsive Design

- Flexible chat container.
- Responsive layout for different screen sizes.
- Uses CSS Flexbox for alignment.

### 9. Tab Notifications

The application supports the following communication events:

| Event | Description |
|---|---|
| USER_JOINED | Notifies connected tabs when a tab joins |
| USER_LEFT | Notifies connected tabs when a tab closes |
| NEW_MESSAGE | Broadcasts a new chat message |
| HEARTBEAT | Announces that a tab is active |

### 10. Lightweight Application

- Developed using Vanilla JavaScript.
- No external frontend framework.
- No backend server required.
- No database required.

---

## 🛠️ Technologies

| Technology | Usage |
|---|---|
| HTML5 | Chat interface structure |
| CSS3 | Styling and animations |
| JavaScript | Application logic |
| BroadcastChannel API | Cross-tab communication |
| DOM API | Dynamic message rendering |

---

## ⚠️ Application Limitations

- Chat works between compatible browser contexts sharing the same origin and storage partition.
- It is not an internet-wide chat service.
- Messages are not permanently stored.
- Chat history disappears when the page is reloaded.
- No user authentication is implemented.
- No database or backend is connected.

---

## 🎯 Learning Outcomes

This project demonstrates practical knowledge of:

- JavaScript Event Handling
- DOM Manipulation
- Browser Communication APIs
- CSS Flexbox
- Responsive Web Design
- Real-Time Interface Updates

---

## 👨‍💻 Developer

**GitHub:** sagarmeena004

**Project:** Live Chat Application

**Technology Stack:** HTML, CSS, JavaScript