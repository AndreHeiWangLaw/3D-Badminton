# 🏸 Badminton 3D Project (OpenGL)

## Project Overview
This repository contains a 3D computer graphics application built using **OpenGL 4.1+** and **GLFW**. The project was developed as part of **COMP 371: Computer Graphics (Summer 2023)** at **Concordia University**. 

Building upon baseline framework mechanics, this application renders a virtual 3D environment featuring a $78\times36$ ground grid enclosed within a massive sky-blue skybox cube. The scene features a modeled tennis/badminton net positioned in the middle of the grid alongside four distinct rackets. Each racket features a uniquely colored character designed from the user's name (`W`, `A`, `L`, `G`) rendered in a retro digital style hovering slightly above it.

---

## 🎮 Controls Guide

### 🎥 Select Racket & Camera Views
Pressing keys `1` through `4` changes both the focus of your camera and selects the active racket model.
* `1` : Focuses 1st person view on **Racket 1** (Character: **W**) *(Default Active)* 
* `2` : Focuses 1st person view on **Racket 2** (Character: **A**) 
* `3` : Focuses 1st person view on **Racket 3** (Character: **L**) 
* `4` : Focuses 1st person view on **Racket 4** (Character: **G**) 
* `5` : Switch to **World View 1** *(The last selected racket 1-4 remains active)*
* `6` : Switch to **World View 2** *(The last selected racket 1-4 remains active)*

### 📐 Model Scaling (Active Racket & Character)
* `u` : Scale model **Up** (Increase size)
* `j` : Scale model **Down** (Decrease size)

### 🏃 Model Translation (Movement)
* `w` : Move **Up** along the Y-axis
* `a` : Move **Left** along the X-axis
* `s` : Move **Down** along the Y-axis
* `d` : Move **Right** along the X-axis

### 🔄 Model Rotation
The character models rotate natively alongside their corresponding rackets:
* **Z-Axis Rotation:**
  * `q` : Rotate **Left**
  * `e` : Rotate **Right**
* **Y-Axis Rotation (Clockwise/Anti-Clockwise):**
  * `z` : Rotate **Left** 
  * `c` : Rotate **Right** 

### 🌍 World Camera Orientation & Zoom
* `Left Arrow` / `Right Arrow` : Orientate camera left / right
* `Up Arrow` / `Down Arrow` : Orientate camera up / down
* `Home` : **Reset** world view orientation to default
* **Mouse Interactions:**
  * `Middle Click + Drag Up/Down` : **Tilt** camera
  * `Right Click + Drag Left/Right` : **Pan** camera
  * `Left Click + Drag In/Out` : **Zoom** out / zoom in

### 🎨 Rendering Modes
Seamlessly alter how the geometric structures are visualized on screen:
* `p` : **Points** mode (Vertices only)
* `l` : **Line** mode (Wireframe display)
* `t` : **Triangle** mode (Fully filled polygons)

### ❌ Program Termination
* `Esc` : Close application window safely

---

### Demo Video
https://github.com/user-attachments/assets/2ad27555-4233-43b1-a9c8-763e036b2cb8

## 🛠️ Technical Specifications
* **Graphics API:** OpenGL 4.1+ (Core Profile) 
* **Windowing & Input:** GLFW 
* **Buffering:** Double buffering enabled for smooth animation tracking 
* **Depth Testing:** Perspective projection view utilizing hidden surface removal (depth testing)
