# 🎠 CSS-Only 3D Image Carousel Slider

A fully responsive **3D image carousel** built **entirely with HTML and CSS** — no JavaScript required. The carousel utilizes CSS variables, transforms, and animations to create an interactive rotating image gallery that runs smoothly and efficiently across modern browsers.

![Preview]
<img width="1914" height="933" alt="Screenshot 2025-07-31 204219" src="https://github.com/user-attachments/assets/539e27a5-c7b1-45a4-bf97-9901b01621c2" />



## 🚀 Features

- ✅ **Pure HTML and CSS** – no JavaScript used at all
- 🎡 3D Carousel effect using `rotateY` and `translateZ`
- 🌈 Smooth infinite rotation via `@keyframes`
- 🔁 Customizable with CSS variables like `--position` and `--quantity`
- 💎 Stylish and modern aesthetic
- 📱 **Responsive design** – works across screen sizes
- ⚡ Lightweight and performance-friendly

---

## 🧩 How It Works

### 📌 Core Logic:
Each carousel item (image) is positioned around a circle using the following CSS formula:

```css
transform: rotateY(calc((var(--position) - 1) * (360 / var(--quantity)) * 1deg))
           translateZ(550px);
🎞️ Animation:
@keyframes autoRun {
    from {
        transform: perspective(1500px) rotateX(-16deg) rotateY(0deg);
    }
    to {
        transform: perspective(1500px) rotateX(-16deg) rotateY(360deg);
    }
}

📁 File Structure
/carousel-slider/
├── index.html         # Main HTML structure
├── style.css          # Carousel styles and animations
└── assets/            # Image files used in the carousel

📱 Responsive Design
The layout adjusts for:
Desktops
Tablets
Mobile devices
Thanks to flexible vw, vh, and transform settings.

🛠️ Customization
You can easily modify:
The number of images: adjust --quantity
Carousel speed: change animation duration
3D depth: modify translateZ value
Tilt: adjust rotateX

📸 Credits
All images used are for demonstration purposes only and belong to their respective creators.

🧑‍💻 Author
Developed by [Avi Varshney]

🌐 Live Preview
Coming soon... (Optional: Add GitHub Pages or Vercel/Netlify link)

📜 License
This project is open source and available under the MIT License.

