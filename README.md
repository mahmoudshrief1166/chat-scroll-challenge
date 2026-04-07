# Chat Auto-Scroll Challenge

## Setup

1. Get a free Gemini API key from [ai.google.dev](https://ai.google.dev)
2. Run `flutter pub get`
3. Run `flutter run` (web, macOS, or any platform)
4. Enter your API key and start chatting

🛠 Features
💬 Flutter Chat UI
Built using flutter_chat_ui and flyer_chat_* packages.
⚡ Streaming Messages
Real-time response streaming from Gemini AI.
🖼️ Image Attachments
Pick and send images from gallery.
🔽 Smart Auto-Scroll
Auto-scrolls only when user is at bottom
Stops auto-scroll when user scrolls up
Resumes automatically when user returns to bottom
✍️ Custom Composer
Multi-line input (1–3 lines)
Shift + Enter to send
Stop button during streaming
⚡ Auto-Scroll Logic (Core Challenge)

The app handles complex scroll behavior similar to modern chat apps:

Detects user position using ScrollController
Prevents unwanted scroll jumps
Handles streaming updates without breaking UX
Maintains smooth scrolling experience
🔧 Recent Fixes & Improvements
✅ Auto-scroll Fix
Introduced _isAutoScrollEnabled and _userScrolledUp
Scroll only triggers when user is at bottom
Prevents forced scroll during reading
✅ Accurate Scroll Detection
Uses scroll position instead of scroll direction
Works even when user is not actively scrolling
✅ Streaming Stability
Messages stream chunk-by-chunk
Safe handling of async updates
Added stop streaming functionality
✅ Composer Enhancements
Dynamic height measurement
Improved keyboard handling
Better UX for message sending


🌐 Live Demo

👉 https://chat-challenge1.netlify.app/

🎥 Screen Recordings
📌 Scenario 1 (Basic Auto-Scroll)
https://drive.google.com/drive/folders/115Xrvju9ub4B1ipqqyoy0Xz7VGiHY0SD
📌 Scenario 2 (Pause on Manual Scroll)
https://drive.google.com/drive/folders/1IvlKsSwqYmdg__tPZ8fImivR7xfZ27v8
📌 Scenario 3 (Send While Scrolled Up)
https://drive.google.com/drive/folders/1Ncf9OoG_jSttjy5X_ZQyknwAPQ6qesmc
📌 Scenario 4 (Resume Auto-Scroll After Scroll Down)
https://drive.google.com/drive/folders/1m1j-ajxBR_1F29wcHV-4PZpuLDPzZSlf

