# 🗺️ Mapty — Map Your Workouts

![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow)
![Status](https://img.shields.io/badge/Status-Completed-success)
![License](https://img.shields.io/badge/License-Learning-blue)

A workout tracking application built while learning modern JavaScript concepts, Object-Oriented Programming, and application architecture.

Users can log running and cycling workouts directly on an interactive map using geolocation. The app stores workouts in local storage and displays them both on the map and in a workout list.

---

## 🚀 Live Demo

Visit the live app here: [tagore-mapty.vercel.app](https://tagore-mapty.vercel.app/)

---

## 📸 Screenshots

![preview](./images/project%20preview/image.png)

### Application Architecture

**_Workflow:_**
![Workflow](./images/Project%20Plan/Mapty-flowchart.png)

**_Architecture part-1:_**
![Architecture-part-1](./images/Project%20Plan/Mapty-architecture-part-1.png)

**_Architecture final:_**
![Architecture-final](./images/Project%20Plan/Mapty-architecture-final.png)

---

# ✨ Features

- 📍 Get current location using Geolocation API
- 🗺️ Interactive map using Leaflet.js
- 🏃 Add Running workouts
- 🚴 Add Cycling workouts
- 📌 Display workout markers on the map
- 📋 Render workout list in sidebar
- 💾 Save workouts in Local Storage
- 🔄 Restore workouts after page reload
- 🎯 Move map to workout location on click
- 🧠 Built using Object-Oriented Programming (OOP)

---

# 🧠 What I Learned

This project helped me understand:

- Modern JavaScript ES6+ features
- Object-Oriented Programming (Classes, Inheritance, Encapsulation)
- Application planning and architecture
- Working with third-party libraries
- Geolocation API
- Local Storage API
- Event handling and DOM manipulation
- Private class fields (`#`)
- Asynchronous JavaScript concepts
- Structuring real-world frontend applications

---

# 🏗️ Project Architecture

The application is built using class-based architecture.

## Core Classes

### `Workout`

Base class containing shared workout properties.

### `Running`

Extends `Workout`

Additional properties:

- cadence
- pace

### `Cycling`

Extends `Workout`

Additional properties:

- elevationGain
- speed

### `App`

Main controller class responsible for:

- Map rendering
- Event handling
- Creating workouts
- Rendering UI
- Local storage management

---

# 🔄 Application Flow

1. User allows location access
2. Map loads using current location
3. User clicks on the map
4. Workout form appears
5. User submits workout details
6. Workout is:
   - Rendered on map
   - Added to sidebar list
   - Saved to local storage
7. Clicking a workout moves map to its location

---

# 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript (ES6+)
- Leaflet.js
- OpenStreetMap
- Geolocation API
- Local Storage API

---

# 📂 Folder Structure

```txt
mapty/
│   .prettierrc
│   index.html
│   README.md
│   script.js
│   style.css
│
└───images
    │   icon.png
    │   logo.png
    │
    ├───Project Plan
    │       Mapty-architecture-final.png
    │       Mapty-architecture-part-1.png
    │       Mapty-flowchart.png
    │       next-features.png
    │
    └───project preview
            image.png
```

---

# ⚙️ Installation & Setup

## 1. Clone the repository

```bash
git clone https://github.com/Tagore9930/mapty.git
```

## 2. Navigate into the project

```bash
cd mapty
```

## 3. Open the project

Simply open `index.html` in your browser.

---

# 🧪 How to Use

1. Allow location access
2. Click anywhere on the map
3. Fill in workout details
4. Submit the form by pressing Enter in any input field.
5. Thw workout will appear:
   - On the map
   - In the sidebar list
6. Click a workout in the list to move to its location

---

# 📌 Future Improvements

![future-plan](./images/Project%20Plan/next-features.png)

- ✏️ Edit workouts
- 🗑️ Delete workouts
- 🧹 Delete all workouts
- 📊 Sort workouts
- 🌍 Show all workouts on map
- ☁️ Weather integration
- 📈 Workout statistics
- 🛣️ Draw routes and paths
- 🔎 Geocoding locations

---

# 💡 Key JavaScript Concepts Used

## Classes & Inheritance

```js
class Running extends Workout {}
class Cycling extends Workout {}
```

## Encapsulation with Private Fields

```js
#map;
#workouts = [];
```

## Local Storage

```js
localStorage.setItem('maptyWorkouts', JSON.stringify(this.#workouts));
```

## Geolocation API

```js
navigator.geolocation.getCurrentPosition();
```

---

# 🙌 Acknowledgements

This project was built while learning from:

- Jonas Schmedtmann
- Leaflet.js
- OpenStreetMap

---

# 📜 License

This project is for learning purposes and portfolio showcase.

---

# 👨‍💻 Author

**Tagore Banda**

- GitHub: [link](https://github.com/Tagore9930)
- LinkedIn: [link](https://www.linkedin.com/in/tagore-banda/)
- Portfolio: [link](https://tagore-portfolio.vercel.app/)
- Fiverr: [link](https://www.fiverr.com/s/xX8zELa)

---

⭐ If you like this project, consider giving it a star on GitHub!
