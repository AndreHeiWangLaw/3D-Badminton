# 🏸 Badminton 3D Project (OpenGL)

## Project Overview
This repository contains a 3D computer graphics application built using **OpenGL 4.1+** and **GLFW**. The project was developed as part of **COMP 371: Computer Graphics (Summer 2023)** at **Concordia University**. 

Building upon baseline framework mechanics, this application renders a virtual 3D environment featuring a $78\times36$ ground grid enclosed within a massive sky-blue skybox cube. The scene features a modeled tennis/badminton net positioned in the middle of the grid alongside four distinct rackets. Each racket features a uniquely colored character designed from the user's name (`W`, `A`, `L`, `G`) rendered in a retro digital style hovering slightly above it.

---

## 📂 Project Structure & Location
The project is built on the foundation of Lab 4 and Assignment 1 components:
* **Visual Studio Solution:** `\Lab04\Lab_Framework\VS2017\Labs.sln`
* **Main Source Code:** `\Lab04\Lab_Framework\Source\lab04.cpp`

---

## 🎮 Controls Guide

### 🎥 Select Racket & Camera Views
[cite_start]Pressing keys `1` through `4` changes both the focus of your camera and selects the active racket model[cite: 51, 55].
* [cite_start]`1` : Focuses 1st person view on **Racket 1** (Character: **W**) *(Default Active)* [cite: 55]
* [cite_start]`2` : Focuses 1st person view on **Racket 2** (Character: **A**) [cite: 55]
* [cite_start]`3` : Focuses 1st person view on **Racket 3** (Character: **L**) [cite: 55]
* [cite_start]`4` : Focuses 1st person view on **Racket 4** (Character: **G**) [cite: 55]
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
[cite_start]The character models rotate natively alongside their corresponding rackets[cite: 47]:
* **Z-Axis Rotation:**
  * `q` : Rotate **Left**
  * `e` : Rotate **Right**
* **Y-Axis Rotation (Clockwise/Anti-Clockwise):**
  * [cite_start]`z` : Rotate **Left** [cite: 52]
  * [cite_start]`c` : Rotate **Right** [cite: 52]

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
* [cite_start]**Graphics API:** OpenGL 4.1+ (Core Profile) [cite: 57]
* [cite_start]**Windowing & Input:** GLFW [cite: 35]
* [cite_start]**Buffering:** Double buffering enabled for smooth animation tracking [cite: 35]
* [cite_start]**Depth Testing:** Perspective projection view utilizing hidden surface removal (depth testing) [cite: 37]
