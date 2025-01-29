# 🔐 SafeChat: Secure Group Messaging with Real-Time Bullying Detection

## 📌 Project Overview
SafeChat is a **secure group messaging platform** designed to detect **real-time bullying** while preserving user privacy. The project integrates **homomorphic encryption** for encrypted sentiment analysis and **AES encryption** for privacy retention.

## 🎯 Features
- 🛡 **Real-Time Bullying Detection** using **NLTK’s VADER Sentiment Analysis**.
- 🔒 **Homomorphic Encryption (TenSEAL)** to analyze messages without decrypting them.
- 🔑 **AES Encryption** to ensure unmatched data security.
- ⚡ **Optimized Processing** to maintain fast message delivery and analysis.
- 🎨 **Gradio App** for an interactive messaging interface in **Google Colab**.

---

## 🔧 Installation & Setup
### 1️⃣ Clone the Repository
```sh
 git clone https://github.com/yourusername/SafeChat.git
 cd SafeChat
```

### 2️⃣ Install Dependencies
```sh
pip install tenseal nltk cryptography gradio flask
```

### 3️⃣ Run the SafeChat Gradio App (in Google Colab)
```python
import gradio as gr
from safechat import start_chat

demo = gr.Interface(fn=start_chat, inputs=["text"], outputs=["text"])
demo.launch()
```

---

## 🔬 How It Works
### **1️⃣ Homomorphic Encryption (TenSEAL)**
- Messages are encrypted before sending.
- Sentiment analysis is **performed on encrypted messages**.
- No plaintext messages are exposed to the server.

### **2️⃣ Real-Time Sentiment & Bullying Detection**
- Uses **NLTK’s VADER Sentiment Analysis**.
- Detects toxic or bullying messages **without decrypting them**.
- Alerts users if a message is flagged as bullying.

### **3️⃣ Secure Message Exchange with AES Encryption**
- **AES encryption** ensures message security.
- Messages remain **fully encrypted in storage and transmission**.

### **4️⃣ Gradio App for Easy Access**
- Built using **Gradio** to provide an interactive UI.
- Hosted directly in **Google Colab** for easy deployment and testing.

---

## 🚀 Performance & Security
### **🛠 Optimizations**
- **Reduced Processing Time** with efficient encryption & sentiment detection.
- **Lightweight Model** for fast real-time message analysis.
- **High Scalability** for multiple users in group chat environments.

---

## 🤝 Contributing
Want to improve SafeChat? Open an issue or submit a pull request. Contributions are welcome! 🚀
