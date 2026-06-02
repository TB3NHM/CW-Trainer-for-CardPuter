# M5Cardputer CW Trainer (TB3NHM)

An interactive, portable Morse Code (CW) trainer developed for the **M5Stack Cardputer**. This tool is designed for amateur radio operators (Hams) to practice listening, sending, and mastering common CW abbreviations and prosigns on the go.

## 🚀 Features

- **Four Specialized Modes:**
  1. **Listening Mode:** The device plays a random character in Morse code; you must identify and input it using the keyboard.
  2. **Sending Mode:** Practice your timing by sending Morse code using dedicated keys (`Z` for Dit, `M` for Dah).
  3. **Abbreviation Challenge:** An interactive quiz using the **CWops** standard list. Listen to the abbreviation (e.g., `QRP`, `73`, `CQ`) and type the answer.
  4. **Free Mode (TX):** A "sandbox" mode where you can type full sentences in Morse code. It decodes and displays your text on the screen in real-time.
- **Optimized UI:** Fully centered text and high-contrast colors designed specifically for the Cardputer's 1.14" TFT screen.
- **Audio Feedback:** Real-time 700Hz tone generation using the Cardputer's built-in speaker.
- **Portable Practice:** No external paddles required—uses the physical keyboard for input.

## 🛠 Hardware Requirements

- **M5Stack Cardputer** (ESP32-S3 based)
- (Optional) MicroSD Card if using with **M5Launcher**

## 💻 Installation

### Option 1: Arduino IDE (Recommended)
1. Install the [ESP32 Board Manager](https://espressif.github.io/arduino-esp32/package_esp32_index.json) in Arduino IDE.
2. Select **M5Stack StampS3** as your board.
3. Install the following libraries via Library Manager:
   - `M5Cardputer`
   - `M5Unified`
4. Set **USB CDC On Boot** to **Enabled** in the Tools menu.
5. Copy the code from `CW_Trainer.ino` and hit **Upload**.

### Option 2: M5Launcher
1. Compile the code to a `.bin` file.
2. Copy the `.bin` file to your SD card.
3. Launch it directly from the **M5Launcher** interface.

## 🎮 How to Use

- **Navigation:** Use the `.` (period) key to scroll through the menu and `Enter` to select a mode.
- **Morse Input:** - `Z` key = **Dit** (.)
  - `M` key = **Dah** (-)
- **Confirmation:** Press `Enter` to decode a character or confirm an answer.
- **Go Back:** Press `Backspace` at any time to return to the main menu.
- **Space:** Use the `Spacebar` in **Free Mode** to add gaps between words.

## 📚 Credits & Standards

- **Abbreviations:** Sourced from the [CWops Abbreviations List](https://cwops.org/).
- **Developer:** Hüseyin EROL, TB3NHM
- **Hardware:** Powered by [M5Stack](https://m5stack.com/).

## ⚖️ License
This project is open-source and available under the MIT License.
