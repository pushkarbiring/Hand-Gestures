# ✨ GPU Gesture Particles 🖐️

A high-performance, interactive 3D particle system running directly in your browser, controlled by real-time hand gestures. 

This project demonstrates how to combine advanced WebGL rendering (Three.js with custom GLSL shaders) with lightweight Machine Learning (Google MediaPipe Hands) to create a futuristic, sci-fi aesthetic inspired by Marvel's *Iron Man* or *Doctor Strange*.

## 🌟 Key Features

* **Real-time Hand Tracking:** Uses the device's front-facing camera to track a single hand in 3D space.
* **Gestural Controls:**
    * 🖐️ **Open Hand:** Expands the entire particle swarm (Scales up).
    * ✊ **Closed Fist:** Contracts the swarm (Scales down) and triggers a shifting neon color palette.
    * 🤏 **Pinch (Thumb + Index):** Cycles between 4 mathematical templates.
* **4 Distinct Templates:** Morph between a **Sphere**, **Heart**, **Flower**, and **Saturn** shape.
* **Neon Glow Aesthetic:** Utilizes Three.js `EffectComposer` and `UnrealBloomPass` for stunning glowing post-processing effects.
* **Highly Optimized (Mobile Ready):** * Draws **10,000 particles** at 60fps on modern smartphones.
    * **Crucial Performance Note:** Unlike basic JavaScript implementation, this version offloads the heavy particle morphing interpolation (`mix`) and gentle drifting physics entirely to a custom **GLSL Vertex Shader** running on the GPU.

## 🛠️ Tech Stack

* [Three.js r128](https://threejs.org/) (WebGL core library)
* Google [MediaPipe Hands v0.4](https://google.github.io/mediapipe/solutions/hands.html) (Computer Vision)
* Custom GLSL Shaders (Vertex & Fragment)

## ⚠️ Important Prerequisites (Run Locally)

Browsers have strict security restrictions regarding camera access. Due to these restrictions, **you cannot run this project by opening the file directly from your storage (`file:///index.html`).**

You must run the project in a **Secure Context**, which means serving it over `https://` or `http://localhost`.

### Easy ways to run locally:
1.  **VS Code:** Install the "Live Server" extension, then right-click `index.html` and choose "Open with Live Server".
2.  **Node.js:** Run `npm install -g http-server` and then `http-server` in the project directory.
3.  **Hosting:** Upload the `index.html` file to free hosts like GitHub Pages, Vercel, or Netlify for automatic HTTPS.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support 💖

If you found this project helpful or just want to support a fellow developer's coding journey, I'd really appreciate it!

[![Buy Me A Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/mrpusu)

[![PayPal](https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://paypal.me/PushkarBiring)

Your support helps me continue building open-source projects and learning AI/ML. 🚀

⭐ If you like this project, consider giving it a star!
