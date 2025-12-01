markdown
# Pixel Rearranger (HD Export)

A browser-based tool that animates pixels from one image to reconstruct another image, inspired by the "Obama pixel animation" style.  
It supports **live preview**, **HD video export**, and **high-resolution image output** — all directly inside your browser.

---

## ✨ Features

✅ Pixel-to-pixel animation  
✅ Live preview mode (fast)  
✅ HD video export (WebM)  
✅ PNG image export  
✅ Resolution selector (720 / 1024 / 1440)  
✅ FPS selector (30 / 60)  
✅ Automatic protection against browser lag  
✅ Fully offline – no server required  

---

## 🖼 How It Works

You upload:

- **Base image** – where pixels are taken from  
- **Target image** – final image to generate  

The tool divides both images into a grid and moves each pixel tile from the base image to its matching color position in the target image.

---

## 🚀 Usage

### 1️⃣ Open the file

Open the HTML file in a modern browser:
- ✅ Chrome
- ✅ Edge
- ✅ Brave  
(Not recommended on mobile)

---

### 2️⃣ Select Images

- Upload a **Base image**
- Upload a **Target image**

---

### 3️⃣ Choose Settings

- **Grid Size**  
  Controls detail level  
  - 48–100 = good balance  
  - 120+ = heavy  
  - 400+ = image-only mode

- **Duration**  
  Animation time in seconds

- **Export Resolution**
  Select output quality

- **FPS**
  Video smoothness

---

### 4️⃣ Preview Animation

Click:

```

Preview

```

This plays the animation directly in the browser.

---

### 5️⃣ Export Video (HD)

Click:

```

Render & Download Video

```

The app records the animation and automatically shows:

```

⬇ Download Video

```

You get a `.webm` HD video file.

---

### 6️⃣ Download Final Image

After preview or export:

```

🖼 Download Image

```

Saves the final image as a PNG.

---

## 🔥 Smart Performance Rules

To avoid crashing your browser:

### ✅ Preview clamping
Preview auto-reduces grid above 120.

### ✅ Image-only mode

If:

```

Grid Size > 400

````

Then:
- ❌ No animation
- ❌ No video
- ✅ Instant final image render only

---

## 📁 Example Output

- `animation_hd.webm` → HD video  
- `final_image.png` → Result image  

---

## 🎞 Convert to MP4 (Optional)

Convert WebM to MP4 using ffmpeg:

```bash
ffmpeg -i animation_hd.webm -movflags faststart output.mp4
````

---

## ⚠ Tips for Best Results

* Use desktop browser
* Do not switch tabs during export
* Lower grid if export is slow
* Higher resolution = longer render time

---

## 🛠 Built With

* HTML5 Canvas
* JavaScript
* MediaRecorder API

---

## 📌 Future Ideas

You can expand this tool with:

* GIF export
* Face auto-detection
* Color profiles
* 4K rendering
* Offline frame rendering
* Upscaler
* FFmpeg batch exporter

---

## 📜 License

Free to use and modify.

---

Enjoy creating pixel animations 🚀

```
