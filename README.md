
# 🧩 ChatTool — Python Socket-Based Chat Application

This is a **terminal-based real-time chat application** built using Python's `socket` and `threading` modules. It supports multiple clients, admin privileges, and moderation commands such as kicking and banning users.

---

## 📌 Features

- Multiple clients can join the chat simultaneously.
- Nickname selection for every user.
- Admin login with a password for special privileges.
- **Admin Commands**:
  - `/kick <nickname>` — remove a user from chat.
  - `/ban <nickname>` — ban a user permanently.
- Banned users are stored in `ban.txt`.
- Real-time broadcasting of messages.

---

## ⚙️ Requirements

- Python 3.x  
- No external libraries required — uses only built-in Python modules.
