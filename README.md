# 🚀 Chat Auto-Scroll Challenge

An advanced chat application built with **Flutter** and **Gemini AI**, focusing on seamless User Experience (UX) through a smart auto-scroll system and real-time message streaming.

---

## 🛠 Features

* **💬 Professional Chat UI:** Built using `flutter_chat_ui` and `flyer_chat_*` packages for a native feel.
* **⚡ Streaming Messages:** Real-time response streaming from Gemini AI, displaying text as it's generated.
* **🖼️ Image Attachments:** Seamlessly pick and send images from your gallery.
* **🔽 Smart Auto-Scroll:** * Auto-scrolls only when the user is already at the bottom.
    * Instantly pauses auto-scroll if the user manually scrolls up to read previous messages.
    * Automatically resumes when the user returns to the bottom.
* **✍️ Custom Composer:** * Multi-line input support (1–3 lines).
    * `Shift + Enter` shortcut to send.
    * Dedicated **Stop** button to interrupt AI streaming.

---

## ⚡ The Auto-Scroll Logic (Core Challenge)

The app solves complex scroll behaviors common in modern chat applications:
* **Position Detection:** Uses `ScrollController` to track the user's exact position.
* **Anti-Jump Logic:** Prevents unwanted layout shifts during streaming updates.
* **Smooth UX:** Maintains a fluid scrolling experience even during high-frequency data updates.

---

## 🔧 Recent Fixes & Improvements

| Feature | Description |
| :--- | :--- |
| **Auto-scroll Fix** | Introduced `_isAutoScrollEnabled` and `_userScrolledUp` flags for precision control. |
| **Accurate Detection** | Uses scroll position thresholds rather than just scroll direction. |
| **Streaming Stability** | Safe handling of asynchronous updates and chunk-by-chunk rendering. |
| **Composer UX** | Dynamic height measurement and improved software keyboard handling. |

---

## 🚀 Getting Started

1.  **Get an API Key:** Obtain a free Gemini API key from [ai.google.dev](https://ai.google.dev).
2.  **Install Dependencies:**
    ```bash
    flutter pub get
    ```
3.  **Run the App:**
    ```bash
    flutter run
    ```
    *(Supports Web, macOS, Android, and iOS)*
4.  **Start Chatting:** Enter your API key in the app and you're good to go!

---

## 🌐 Live Demo

🔗 [Check out the Live Demo here](https://chat-challenge1.netlify.app/)

---

## 🎥 Screen Recordings (Scenarios)

* 📌 **Scenario 1:** [Basic Auto-Scroll](https://drive.google.com/drive/folders/115Xrvju9ub4B1ipqqyoy0Xz7VGiHY0SD)
* 📌 **Scenario 2:** [Pause on Manual Scroll](https://drive.google.com/drive/folders/1IvlKsSwqYmdg__tPZ8fImivR7xfZ27v8)
* 📌 **Scenario 3:** [Send Message While Scrolled Up](https://drive.google.com/drive/folders/1Ncf9OoG_jSttjy5X_ZQyknwAPQ6qesmc)
* 📌 **Scenario 4:** [Resume Auto-Scroll After Scrolling Down](https://drive.google.com/drive/folders/1m1j-ajxBR_1F29wcHV-4PZpuLDPzZSlf)

---
✨ Developed with passion using **Flutter** and **Google Gemini AI**.
