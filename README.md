📸 Perspective Projection & Pinhole Camera SimulatorThis project implements a 3D-to-2D perspective projection engine from scratch using Python and NumPy. It simulates how a pinhole camera perceives a 3D world, specifically visualizing a unit cube through different camera orientations and positions.
🚀 Key Features
World-to-Camera Transformation: Implemented coordinate system shifts using rotation matrices ($R$) and translation vectors ($t$).
Pinhole Projection Logic: Applied central projection formulas to map 3D points onto a 2D image plane based on focal length ($f$).
Dynamic Visualization: Used Matplotlib to create side-by-side comparisons of the 3D scene and the resulting 2D image. 
Coordinate System Handling: Visualized world axes (X, Y, Z) within the projected frame to verify orientation accuracy.

🛠 Tech Stack

Language: Python 
Math: NumPy (Matrix operations, Orthogonal transformations) 
Visualization: Matplotlib (3D & 2D plotting)

📈 Results
The simulation demonstrates how parallel lines in 3D space converge at vanishing points in 2D, a fundamental concept in Machine Vision and 3D Rendering.
