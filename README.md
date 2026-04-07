# Chat Auto-Scroll Challenge

## Setup

1. Get a free Gemini API key from [ai.google.dev](https://ai.google.dev)
2. Run `flutter pub get`
3. Run `flutter run` (web, macOS, or any platform)
4. Enter your API key and start chatting

## 🛠 Features

- **Flutter Chat UI**: Custom UI using `flutter_chat_ui` and `flyer_chat_*` packages.
- **Streaming Messages**: Supports real-time text streaming from Gemini AI.
- **Image Attachments**: Users can attach images from the gallery.
- **Auto-scroll Behavior**:
  - Scrolls automatically to the bottom **only if the user hasn't scrolled up**.
  - Detects if the user has scrolled up to prevent jumping down while reading.
- **Custom Composer**:
  - Multi-line text input (1–3 lines)
  - Shift+Enter to send messages
  - Stop button while streaming

---

## ⚡ Recent Updates / Fixes

1. **Auto-scroll fix**:
   - `_isAutoScrollEnabled` and `_userScrolledUp` flags added.
   - Chat only scrolls to bottom if the user is at the bottom.
   - Prevents chat from jumping to bottom when user is reading older messages.

2. **Scroll detection**:
   - `_isBottom` and `_isNoBottom` getters track scroll position accurately.
   - `_scrollController` listener updates scroll behavior in real time.

3. **Streaming messages handling**:
   - `_sendContent` handles text streaming and inserts messages progressively.
   - Proper cancellation using `_stopCurrentStream()`.

4. **Composer improvements**:
   - Handles multi-line input with Shift+Enter
   - Dynamically measures height for proper positioning
   - Stops stream or sends message depending on state

---


### Deployed URL

[Live Demo]([https://your-deployed-url.com](https://chat-challenge1.netlify.app/))

### Screen Recordings

- **Scenario 1 (Basic Auto-Scroll):** [Watch Recording]([https://your-recording/scenario1](https://drive.google.com/drive/folders/115Xrvju9ub4B1ipqqyoy0Xz7VGiHY0SD?usp=drive_link))
- **Scenario 2 (Pause on Manual Scroll):** [Watch Recording]([https://your-hrecording/scenario2](https://drive.google.com/drive/folders/1IvlKsSwqYmdg__tPZ8fImivR7xfZ27v8?usp=drive_link))
- **Scenario 3 (Send While Scrolled Up):** [Watch Recording]([https://your-recording/scenario3](https://drive.google.com/drive/folders/1Ncf9OoG_jSttjy5X_ZQyknwAPQ6qesmc?usp=drive_link))
- **Scenario 4 (Resume Auto-Scroll After Scroll Down):** [Watch Recording]([https://your-recording/scenario4](https://drive.google.com/drive/folders/1m1j-ajxBR_1F29wcHV-4PZpuLDPzZSlf?usp=drive_link))
 

