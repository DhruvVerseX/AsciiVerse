# ASCII-Motion: Your Terminal, Your Cinema

**Transform any video into a vibrant ASCII art performance right in your terminal.**

ASCII-Motion is a Python-based video player that brings a unique, retro-artistic twist to your viewing experience. It meticulously converts video frames into colorful ASCII characters, rendering them in real-time to create a smooth, captivating playback.

---

### 🎬 Key Features

- **Universal Video Compatibility**: If OpenCV can read it, ASCII-Motion can play it.
- **Full-Color ASCII Art**: Retains the original RGB colors of the video, mapping them to each ASCII character.
- **Responsive Terminal Playback**: Automatically detects and adjusts to your terminal's dimensions for an optimal viewing area.
- **Interactive Playback Controls**:
  - **Play/Pause**: Toggle with the `Spacebar`.
  - **Adjust Speed**: Use the `←` and `→` arrow keys to slow down or speed up the video.
  - **Quit**: Exit the player instantly with `q` or `Q`.
- **Smooth Performance**: A multi-threaded engine processes video frames in the background to prevent stuttering and ensure a seamless playback experience.
- **Real-time Speed Indicator**: A discreet on-screen display shows the current playback speed (e.g., `1.0x`, `2.0x`, `paused`).

---

### 🚀 Getting Started

Follow these simple steps to get ASCII-Motion up and running.

**1. Prerequisites**
- Ensure you have Python 3.7 or newer installed.

**2. Clone the Repository**
```bash
git clone https://github.com/manthanawgan/ascii-motion.git
cd ascii-motion
```

**3. Install Dependencies**
A `requirements.txt` file is included to manage all necessary libraries.
```bash
pip install -r requirements.txt
```

---

### ▶️ How to Use

To start the player, simply run the main script with the path to your video file as an argument.

```bash
python main.py <path_to_your_video>
```

**Example:**
```bash
python main.py my_video.mp4
```

---

### 🎨 The ASCII Conversion Process

The magic of ASCII-Motion lies in its character mapping. The script analyzes each pixel's brightness in a video frame and substitutes it with a corresponding character from a predefined density table. This creates the illusion of shades and shapes. The darkest pixels are replaced by characters like `@` and `#`, while the brightest are represented by `.` and `'`.

The density table used is:
```
     .'`^",:;Il!i><~+_-?][}{1)(|\/tfjrxnuvczXYUJCLQ0OZmwqpdbkhao*#MW&8%B@$
```

---

### 📄 License

This project is open-source and distributed under the MIT License. See the `LICENSE` file for more details.