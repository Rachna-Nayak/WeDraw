# 🖊️ WeDraw - Secure Collaborative Whiteboard

WeDraw is a real-time collaborative whiteboard application built in Python using `Tkinter` for the GUI and `SSL` sockets for secure client-server communication. Multiple users can draw simultaneously and see each other's changes in real-time — all over a secure encrypted channel.

---

## 🚀 Features

- 🎨 Drawing tools: pen, rectangles, circles, and text
- 🌈 Custom color picker and color wheel
- ↩️ Undo and 🧹 clear all actions
- 🔐 Secure SSL communication between clients and server
- 🔁 Automatic client reconnection on server disconnect
- 💾 Drawing history is replayed for new clients
- 🖥️ Simple GUI built using Tkinter

## 🛠️ Project Structure
├── ssl_client.py # Client GUI with drawing tools and SSL connection <br/>
├── ssl_server.py # Server handling secure communication and broadcasting <br/>
├── certificate.pem # SSL certificate (public) <br/>
├── key.pem # SSL private key <br/>
└── README.md

## 📦 Requirements

- Python 3.8+
- Tkinter (usually pre-installed)
- Pillow (`pip install pillow`)

## How to Run 
- Start the server:
    - Linux: python3 ssl_server.py
    - Windows: python ssl_server.py
- Start the client:
    - Linux: python3 ssl_client.py
    - Windows: python3 ssl_client.py
 
## 📋 Customization
- Change drawing colors, shapes, or add your own tools in ssl_client.py
- Improve SSL settings (like client auth) for production
- Deploy over LAN or configure for internet use (port forwarding + domain + real cert)
