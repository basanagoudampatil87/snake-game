# 🐍 Snake Game

A modern neon-style **Snake Game** built using **HTML, CSS, and JavaScript**.  
This project features smooth gameplay, dark UI aesthetics, responsive controls, score tracking, and keyboard navigation.

---

# 🎮 Preview

## Main Interface

<img width="1200" height="900" alt="collage" src="https://github.com/user-attachments/assets/08f5b908-447b-4218-83a9-75b08e5fecf9" />


---

# ✨ Features

- 🎯 Real-time score tracking
- 🚀 Increasing difficulty levels
- 🎨 Modern neon dark UI
- ⌨️ Keyboard controls
- 📱 Responsive design
- 🔁 Restart & Pause buttons
- 🕹️ Arrow key controls on screen
- 💀 Game Over detection

---

# 🛠️ Technologies Used

| Technology | Usage |
|------------|-------|
| HTML5 | Structure |
| CSS3 | Styling & Animations |
| JavaScript | Game Logic |

---

# 📂 Project Structure

```bash
snake-game/
│
├── index.html
├── style.css
├── script.js
└── assets/
    └── preview.png
```

---

# 🚀 Getting Started

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/snake-game.git
```

---

## 2️⃣ Open Project

```bash
cd snake-game
```

---

## 3️⃣ Run the Game

Simply open:

```bash
index.html
```

in your browser.

---

# 🎮 Controls

| Key | Action |
|-----|--------|
| ⬆️ Arrow Up | Move Up |
| ⬇️ Arrow Down | Move Down |
| ⬅️ Arrow Left | Move Left |
| ➡️ Arrow Right | Move Right |

---

# 📸 UI Showcase

## Neon Dark Theme

```css
body{
    background:#050505;
    color:#7c6cff;
    font-family: 'Poppins', sans-serif;
}
```

---

## Snake Styling

```css
.snake{
    background: linear-gradient(45deg,#7c6cff,#9a8cff);
    border-radius:4px;
}
```

---

## Food Styling

```css
.food{
    background:#ff6b35;
    border-radius:50%;
}
```

---

# 🧠 Core JavaScript Logic

## Snake Movement

```javascript
function moveSnake() {

    const head = {
        x: snake[0].x + direction.x,
        y: snake[0].y + direction.y
    };

    snake.unshift(head);

    if(head.x === food.x && head.y === food.y){
        score++;
        generateFood();
    } else {
        snake.pop();
    }
}
```

---

## Collision Detection

```javascript
function checkCollision() {

    const head = snake[0];

    return (
        head.x < 0 ||
        head.y < 0 ||
        head.x >= tileCount ||
        head.y >= tileCount ||
        snake.slice(1).some(
            segment =>
            segment.x === head.x &&
            segment.y === head.y
        )
    );
}
```

---

# 🎨 UI Buttons

```html
<div class="controls">
    <button id="restartBtn">Restart</button>
    <button id="pauseBtn">Pause</button>
</div>
```

---

# 📈 Future Improvements

- 🔊 Sound Effects
- 🏆 High Score Storage
- 🌐 Multiplayer Mode
- 📱 Mobile Swipe Controls
- 🎵 Background Music

---

# 🤝 Contributing

Contributions are welcome!

```bash
Fork → Clone → Edit → Commit → Push → Pull Request
```

---

# 📜 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Your Name**

GitHub: [@your-username](https://github.com/your-username)

---

# ⭐ Support

If you like this project:

⭐ Star the repository  
🍴 Fork the project  
📢 Share with friends

---

# 🐍 Game Over Screen Example

```javascript
if(checkCollision()){
    gameOver = true;
    alert("Game Over!");
}
```

---

# 🔥 Final Output

✔ Modern UI  
✔ Smooth Gameplay  
✔ Responsive Controls  
✔ Beginner Friendly Source Code

---
