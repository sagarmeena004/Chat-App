# 💬 Live Chat Application — Technology Stack

## 📌 Project Overview

Live Chat Application is a frontend-based real-time cross-tab messaging application developed using HTML5, CSS3, and Vanilla JavaScript.

The application uses the BroadcastChannel API to exchange messages between compatible browser tabs without requiring a backend server or database.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling and responsive layout |
| JavaScript | Application functionality |
| BroadcastChannel API | Cross-tab messaging |
| DOM API | Dynamic interface updates |
| Browser Events | User interaction and tab lifecycle |

---

## 1. HTML5

HTML5 is used to create the structure of the Chat Application.

### Components

- Chat header
- Connected tabs information
- Message display area
- Message input field
- Send button
- Application status indicator

### Key HTML Elements

- `<div>` — Layout containers
- `<input>` — Message input
- `<button>` — Send messages
- `<script>` — JavaScript functionality
- `<style>` — CSS styling

---

## 2. CSS3

CSS3 is used to design the chat interface.

### Features

- Responsive layout
- Flexbox alignment
- Rounded message bubbles
- Dark-themed background
- Hover effects
- CSS animations
- Custom scrollbar
- Message alignment

### Important CSS Concepts

- Flexbox
- Border Radius
- Box Shadow
- CSS Transitions
- Keyframe Animations
- Background Images

---

## 3. JavaScript

Vanilla JavaScript handles the application logic.

### Functionalities

- Sending messages
- Receiving messages
- DOM manipulation
- Message timestamps
- Input validation
- Browser event handling
- Tab communication
- Active tab tracking

### JavaScript Concepts

- Functions
- Arrow Functions
- Event Listeners
- Template Literals
- DOM Methods
- Set Data Structure
- Timers
- Conditional Statements
- Switch Statements

---

## 4. BroadcastChannel API

The BroadcastChannel API enables communication between compatible browsing contexts sharing the same origin and storage partition.

### Channel Initialization

```javascript
const channel = new BroadcastChannel('live_chat_frontend');
```

### Sending Messages

```javascript
channel.postMessage({
  type: 'NEW_MESSAGE',
  text: 'Hello!'
});
```

### Receiving Messages

```javascript
channel.onmessage = (event) => {
  console.log(event.data);
};
```

These examples demonstrate the API used by the project.

---

## 5. DOM Manipulation

JavaScript dynamically updates the chat interface.

### Methods Used

- `document.getElementById()`
- `document.createElement()`
- `appendChild()`
- `addEventListener()`
- `innerText`
- `innerHTML`

DOM manipulation allows messages and notifications to appear without refreshing the page.

---

## 6. Browser Events

The application uses browser events to handle user interactions.

| Event | Purpose |
|---|---|
| click | Send messages using the button |
| keypress | Send messages using Enter |
| beforeunload | Notify other tabs when leaving |
| message | Receive BroadcastChannel messages |

---

## 7. Application Architecture

```text
User Input
    |
    v
JavaScript Event Handler
    |
    v
Message Validation
    |
    v
Update Sender Chat UI
    |
    v
BroadcastChannel API
    |
    v
Other Connected Browser Tabs
    |
    v
Update Receiver Chat UI
```

---

## 8. Project Dependencies

This project does not require:

- React
- Angular
- Vue.js
- Node.js
- Express.js
- Database
- External JavaScript libraries

It is developed using native browser technologies.

---

## 9. Technical Limitations

- Messages are not stored permanently.
- No user authentication is implemented.
- No backend communication is available.
- Cross-device messaging is not supported.
- Active tab tracking does not automatically expire all inactive tabs.

---

## 🎯 Learning Outcomes

This project demonstrates:

- Frontend Web Development
- JavaScript Programming
- Browser APIs
- Event-Driven Programming
- Responsive Interface Design
- Cross-Tab Communication

---

## 👨‍💻 Developer

**GitHub:** sagarmeena004

**Project:** Live Chat Application

**Tech Stack:** HTML5, CSS3, JavaScript