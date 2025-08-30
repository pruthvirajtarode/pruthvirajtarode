# 🚗 Romania Search Game (Prolog + XPCE GUI)

This project implements the classic **Romania map search problem** as a **graphical interactive game** using **SWI-Prolog** and its GUI library **XPCE**.  
It allows you to explore search algorithms like **BFS, DFS, Greedy Best-First, and A*** with live **map visualization** and **car animation**.

---

## ✨ Features
- 🎛️ Interactive **menu system** with dropdowns:
  - Select **Start City** and **Goal City**
  - Choose **Algorithm** (BFS, DFS, Greedy, A*)
  - Adjust **Speed** (Slow, Medium, Fast)
  - Toggle **Show Expansions**
- 🗺️ Graphical **map of Romania** (20 cities + roads)
- 🚗 Animated **red car** moving step-by-step along the chosen path
- 🔵 Blue-highlighted path showing the solution
- 🟢 Green markers for **expanded cities**
- 📊 Info panel with:
  - Algorithm name  
  - Start and Goal cities  
  - Path cost  
  - Full path taken  

---

## 🛠️ Requirements
- **SWI-Prolog** (tested with v9.x, includes XPCE GUI)
  - Download: [https://www.swi-prolog.org/Download.html](https://www.swi-prolog.org/Download.html)

---

## ▶️ How to Run
1. Clone/download this repository:
   ```bash
   git clone https://github.com/your-username/romania-prolog-game.git
   cd romania-prolog-game
   ```
2. Open **SWI-Prolog**.
3. Load the project file:
   ```prolog
   ?- ['romania_game_gui.pl'].
   ```
   You should see:
   ```
   true.
   ```
4. Start the game:
   ```prolog
   ?- start_menu.
   ```

---

## 🎮 Example Demo
1. **Start city:** arab  
2. **Goal city:** bucharest  
3. **Algorithm:** A*  
4. **Speed:** slow  
5. **Show expansions:** yes  

👉 You will see:
- 🟢 Green dots = expanded nodes  
- 🔵 Blue path = final solution  
- 🚗 Red car = animated travel from **arab → sibiu → fagaras → bucharest**  
- 📊 Cost and path details in side panel  

---

## 📂 Project Structure
```
romania-prolog-game/
│
├── romania_game_gui.pl   # Main Prolog source code
├── README.md             # Documentation (this file)
├── .gitignore            # Git ignore file
```

---

## 📖 Background
The Romania problem is a classic example in AI, popularized by **Russell & Norvig – Artificial Intelligence: A Modern Approach**.  
It illustrates how different search algorithms behave when solving a navigation problem.

---

## 📹 Demo Preview (Optional for GitHub)
You can record a demo GIF/video showing the game in action:

### Windows (using ShareX)
1. Install [ShareX](https://getsharex.com/).
2. Run the game (`?- start_menu.`).
3. Select start = arab, goal = bucharest, algorithm = astar, slow speed.
4. Use ShareX → **Capture > Screen recording (GIF)**.
5. Save as `demo.gif` inside your repo.

### Linux/Mac
- Use `peek` (Linux) or `ScreenToGif` (Mac alternatives available).
- Save recording as `demo.gif`.

Once recorded, add to your repo and update README:

```markdown
## 🎥 Demo
![Demo GIF](demo.gif)
```

---

## 🙌 Credits
- Developed in **SWI-Prolog** with **XPCE GUI**
- Visualization of the Romania map search problem  
- Inspired by **Artificial Intelligence: A Modern Approach** (Russell & Norvig)
