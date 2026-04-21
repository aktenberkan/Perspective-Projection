# 📸 Perspective Projection & Pinhole Camera Simulator

This project implements a 3D-to-2D perspective projection engine from scratch using **Python** and **NumPy**. It simulates the mathematical principles of the **Pinhole Camera Model**, mapping 3D world coordinates onto a 2D image plane.

## 🚀 Overview

The simulation visualizes a unit cube centered at the world origin and projects it through two different camera configurations:
* **Camera A:** Aligned with the world axes for a frontal view.
* **Camera B:** Positioned at a diagonal angle (`[4, 3, 2]`) to demonstrate complex perspective and vanishing points.

## 🛠 Technical Implementation

### 1. World-to-Camera Transformation
Implemented coordinate system shifts using the following transformation:
$$\mathbf{p}_C = {}^W R_C^\top \cdot (\mathbf{p}_W - {}^W t_C)$$
* **Rotation ($R$):** Orthogonal matrix handling camera orientation.
* **Translation ($t$):** Vector defining the camera's position in the 3D world.

### 2. Central (Pinhole) Projection
Mapped 3D camera-frame points onto the image plane using the focal length ($f = 1$):
$$x_{img} = f \cdot \frac{X_C}{Z_C}, \quad y_{img} = f \cdot \frac{Y_C}{Z_C}$$

### 3. Visualization
* **3D Scene:** Displays the world axes, the cube, and the camera's relative position/orientation.
* **2D Projected Image:** Shows the resulting perspective, where parallel lines in 3D converge at vanishing points in 2D.

## 🧰 Tech Stack
* **Language:** Python
* **Mathematics:** NumPy (Matrix operations, Linear Algebra)
* **Visualization:** Matplotlib (3D & 2D Plotting)

## 📊 Key Results
The project successfully demonstrates:
1. **Perspective Distortion:** Farther edges of the cube appear smaller, mimicking human/camera perception.
2. **Axis Projection:** World X (Red), Y (Green), and Z (Blue) axes are correctly projected as arrows in the image frame.
3. **Pinhole Logic:** Discarding points behind the camera ($Z_c \leq 0$) to ensure physical accuracy.

---
*Developed as part of the Machine Vision curriculum during my Erasmus+ exchange at Tomas Bata University in Zlín.*
