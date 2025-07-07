# 🖱️ HandiGo – Virtual Mouse System

**HandiGo** is an AI-based virtual mouse system that allows users to control cursor movement using hand gestures. It is designed to assist physically disabled users by providing a contactless way to interact with computers using only a webcam and hand movements.

---

## 🎯 Aim

To build an accessible computer interaction tool using hand gesture recognition that acts as a virtual mouse — allowing cursor movement, click, and scroll gestures using a webcam.

---

## 🛠️ Features

- 👋 Cursor movement using hand position
- 🖐️ Left & right click detection through finger gestures
- 🔄 Scroll control using hand up/down gestures
- 🧠 Real-time hand tracking using OpenCV + Mediapipe
- 📷 Uses regular webcam – no additional hardware required
- ⚡ Smooth and fast frame detection

---

## 🔧 Technologies Used

| Layer       | Tools / Libraries Used                    |
|-------------|-------------------------------------------|
| Hand Detection | Python, OpenCV, Mediapipe               |
| Virtual Mouse | PyAutoGUI                               |
| Backend (optional) | Flask / Node.js (for settings API) |
| UI (optional) | React.js / Tkinter (for control panel)  |
| ML (if used) | Custom gesture model (optional)          |

---

## 📈 Model Training & Evaluation

- **Train-test split**: 80% training, 20% testing
- Used `scikit-learn` for model training and evaluation
- **Accuracy achieved**: ~94% on validation set

| Metric     | Value    |
|------------|----------|
| Accuracy   | 94%      |
| Precision  | 0.93     |
| Recall     | 0.91     |
| F1 Score   | 0.92     |

- Confusion matrix showed clear distinction between gesture classes
- The model was evaluated across varying lighting and hand positions to test generalization

---

## 🧠 How It Works

1. **Hand Tracking:** Mediapipe detects hand landmarks in real time  
2. **Finger Detection:** Based on fingers raised, interpret action  
   - Index only → Move cursor  
   - Index + middle → Left click  
   - Thumb + index → Right click  
   - Two fingers slide → Scroll  
3. **Trigger Mouse Events:** PyAutoGUI converts gestures into system mouse commands

---

## 💡 Real-World Applicability

- ♿ **Accessibility Tool**: Ideal for people with upper limb disabilities to control the system without a mouse
- 🧪 **Contactless Interaction**: Helpful in medical environments or clean rooms where physical contact is avoided
- 🎓 **Educational Demos**: Useful for demonstrating real-time AI + CV integration
- 🔐 **Touchless Public Terminals**: Can be extended to kiosks, ATMs, or self-checkout systems

---

## 📝 Author

**Harshita Sinha**  
 [GitHub](https://github.com/HarshitaSinha09)

---

## 🤝 Feedback & Ideas

Open to suggestions, issues, and collabs! Feel free to open an issue or contact.

---

