# 🌍🌙 CSS Moon Orbit Animation (Two Techniques)

This project demonstrates how to simulate the moon orbiting around the Earth using **pure CSS**, implemented in **two different ways**:

1. 🌀 **Container Rotation Method**
2. 🔁 **Transform + Translate Method**

It also includes interactive hover effects and visual enhancements like glow using `box-shadow`.

---

## 🚀 Live Demo

> *(Add your GitHub Pages link here)*

---

## 🎯 Key Features

* 🌍 Earth and 🌙 Moon built with CSS
* 🌀 Orbit using **rotating container**
* 🔁 Orbit using **rotate + translate**
* ⏸️ Pause animation on hover (container method)
* 🐢 Slow motion effect on hover (translate method)
* ✨ Glow effects using `box-shadow`
* 🎨 Space background using `background: url()`

---

## 🛠️ Technologies Used

* HTML5
* CSS3

  * Flexbox
  * CSS Grid
  * `transform` (rotate, translate)
  * `@keyframes` animations
  * CSS variables (`--speed`)
  * `box-shadow`
  * Background images

---

## 🧠 Concepts Demonstrated

### 🌀 1. Container Rotation Method

* The moon is placed inside a rotating parent (`.moon-container`)
* The entire container rotates using `@keyframes spin`
* Hovering pauses the animation:

```css
.moon-container:hover {
  animation-play-state: paused;
}
```

---

### 🔁 2. Transform + Translate Method

* The moon orbits using:

```css
transform: rotate(...) translate(...);
```

* This creates a circular path without needing a parent container

* Hovering slows down the animation dynamically:

```css
.earth2:hover .moon2 {
  --speed: 60s;
}
```

---

## ⚙️ How It Works

* **Method 1:** Rotate a wrapper → moon follows circular path
* **Method 2:** Rotate + translate → creates orbit mathematically
* CSS variables allow dynamic control of animation speed
* `box-shadow` adds glow to simulate light in space

---

## 📂 Project Structure

```
📁 project-folder
│── index.html
│── style.css
│── space.jpg
│── earth.jpg
│── moon.png
```

---

## 📸 Preview

> *(Add a GIF here — highly recommended for animations)*

---

## 💡 What I Learned

* Difference between **rotating a container vs transforming an element**
* How `transform-origin` affects motion
* Creating circular motion using `rotate + translate`
* Controlling animations with CSS variables
* Using hover interactions to modify animation behavior
* Enhancing visuals with `box-shadow` and backgrounds

---

## 🔮 Future Improvements

* Add elliptical orbits (more realistic physics)
* Introduce multiple planets
* Add shadows and lighting effects
* Control speed with UI (slider using JS)
* Add stars animation in the background

---

## 👨‍💻 Author

**Mohamad Aboeisa**

---

## 📄 License

This project is open source and available under the MIT License.
