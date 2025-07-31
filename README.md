# ChatCord

ChatCord is a real-time chat application built with Node.js, Express, and Socket.io. It allows users to join chat rooms, send messages, and see who else is in the room. The app features a simple and clean interface for seamless communication.

## Features

- Real-time messaging using WebSockets (Socket.io)
- Multiple chat rooms support
- User join/leave notifications
- Display of active users in each chat room
- Timestamped messages
- Responsive and user-friendly interface

## Project Structure

```
.
├── Public/                 # Frontend static files
│   ├── CSS/               # Stylesheets
│   ├── JS/                # Client-side JavaScript
│   ├── chat.html          # Chat room page
│   └── index.html         # Landing page / login
├── utils/                 # Utility modules
│   ├── messages.js        # Message formatting utility
│   └── users.js           # User management utility
├── server.js              # Main server file
├── package.json           # Project metadata and dependencies
└── README.md              # Project documentation
```

## Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd ChatBox
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

## Usage

1. Start the server:

   ```bash
   node server.js
   ```

2. Open your browser and navigate to:

   ```
   http://localhost:3000
   ```

3. Enter a username and select a chat room to join.

4. Start chatting in real-time with other users in the same room.

5. To leave the chat room, click the "Leave Room" button.

## Dependencies

- [Express](https://expressjs.com/) - Web framework for Node.js
- [Socket.io](https://socket.io/) - Real-time bidirectional event-based communication
- [Moment.js](https://momentjs.com/) - Date and time formatting
- [Qs](https://github.com/ljharb/qs) - Query string parsing (used on client-side)

## How It Works

- The server serves static files from the `Public` directory.
- When a user connects, they join a specific chat room.
- Messages are sent and received in real-time using Socket.io.
- The server keeps track of users and rooms using utility functions.
- Messages are formatted with timestamps before being broadcast.
- The client updates the chat window and user list dynamically.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the MIT License.
