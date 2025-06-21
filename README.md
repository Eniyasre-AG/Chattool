# chattool
🧩 ChatTool — Python Socket-Based Chat Application
This is a terminal-based real-time chat application built using Python's socket and threading modules. It supports multiple clients, admin privileges, and moderation commands such as kicking and banning users.

📌 Features
Multiple clients can join the chat simultaneously.

Nickname selection for every user.

Admin login with a password for special privileges.

Admin commands:

/kick <nickname> — remove a user from chat.

/ban <nickname> — ban a user permanently.

Banned users are stored in ban.txt.

Real-time broadcasting of messages.

⚙️ Requirements
Python 3.x

No external libraries required — uses only built-in Python modules.

📁 File Structure
arduino
Copy
Edit
chattool/
│
├── server.py       # Server-side script
├── client.py       # Client-side script
├── ban.txt         # (auto-created) list of banned users
├── requirements.txt (optional)
└── README.md       # Documentation
🚀 How to Run
1️⃣ Start the Server
In a terminal:

bash
Copy
Edit
python server.py
This will start the server on 127.0.0.1:55555.

2️⃣ Start a Client
In a new terminal window:

bash
Copy
Edit
python client.py
Enter a nickname when prompted.

If the nickname is admin, you’ll be prompted for a password.

Default admin password is adminpass.

🔐 Admin Commands
After connecting as admin, type:

/kick <nickname> — kicks the user.

/ban <nickname> — bans and kicks the user permanently.

Example:

text
Copy
Edit
/kick john
/ban eve
🧯 Error Handling
Banned users receive a "connection refused" message and cannot reconnect.

Invalid admin passwords are rejected.

Commands from non-admin users are ignored with a warning.

🛑 Important Notes
Do not upload venv/ or any environment files to GitHub.

To recreate the environment, use:

bash
Copy
Edit
pip freeze > requirements.txt
👩‍💻 Contributors
Built by eniya with ❤️ using Python sockets and threads.
