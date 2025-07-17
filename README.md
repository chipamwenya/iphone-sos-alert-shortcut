# 📱 iPhone Emergency SOS Automation (Back Tap Triggered Shortcut)

This project showcases a **semi-automated emergency alert system** built entirely within the iOS ecosystem using the **Shortcuts app**. The goal is to provide users a fast, discreet, and hands-free way to notify trusted contacts when facing sudden or dangerous situations.

---

## 🎯 Purpose

The automation empowers users to trigger a distress message by simply **double-tapping the back of their iPhone** (using Back Tap + Shortcuts). It opens LINE with a pre-filled emergency message, informs the recipient that the user has been stopped by the authorities, and follows up with a phone call — all while **live location sharing via Find My** is active.

---

## 🧠 Problem It Solves

People in distress (e.g., followed, harassed, stopped unfairly by authroities) may not have time to:
- Open their phone
- Navigate to messaging apps
- Type out and send a message

This shortcut:
- Works **hands-free**
- Uses **natural gestures**
- Notifies trusted contacts **quickly and discreetly**

---

## ⚙️ How It Works

1. Triggered by **Back Tap (Double Tap)** gesture
2. Opens LINE app with a **pre-composed emergency message**
3. Message mentions that the user is ** e.g being stopped unfairly, being harrassed or in trouble**
4. Live location is **already shared via Find My**
5. After a short delay, the automation **initiates a call** to the recipient

---

## 🚧 Technical Challenges

### ❌ LINE doesn't support message sending via Shortcuts  
- LINE’s iOS integration doesn’t allow selecting LINE contacts directly.

### ✅ Workaround: URL Scheme  
Used the `line://msg/text/` URL scheme to open LINE with a pre-filled message.

### ✅ Used URL Encoding  
Since messages include line breaks and special characters, a **URL Encoding step** was used to prevent syntax breakage when passed into the LINE URL.

---

## 🧪 Example Use Cases

- Stopped by law enforcement
- Followed in public
- Walking alone at night
- Situations where **only voice or gesture-based activation is possible**

---

## 🔮 Future Applications

- Integration with **Google Maps live location URLs** for Android users
- Use of **LINE Notify API** to fully automate message delivery
- Adding **voice playback**, **flashlight pulse**, or **local alarm**
- Expand to multi-recipient groups or emergency hotlines

---

## 🔐 Privacy Note

Location is only shared **with the specific contact** selected by the user. No one else can access the user’s location.

---

