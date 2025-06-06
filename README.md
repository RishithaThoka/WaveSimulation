# WaveSimulation
This repository contains a physics-computer science project by Rishitha Thoka . It includes a presentation on wave mechanics and an interactive JavaScript wave simulation that oscillates on click or drag, solving the wave equation with damping and stiffness.
# Contents
- WAVES.pdf: Presentation covering wave types, characteristics, and properties.
- index.html: HTML file with canvas for the wave simulation.
- index.js: JavaScript code implementing the wave equation and interactive oscillation.
- wave_equation.ipynb: IPython notebook explaining the wave equation and coordinate conversions.
- LICENSE: MIT License file.
# Project Details
#Presentation (WAVES.pdf)
- Wave Definition: A disturbance carrying energy through a medium.
- Types: Transverse, longitudinal, mechanical, and electromagnetic waves.
- Characteristics: Crest, trough, amplitude, wavelength, frequency, period.
- Properties: Reflection, refraction, diffraction, interference.
- Wave Speed: Calculated as frequency × wavelength.--------------------------
#Simulation (index.html, index.js):
An interactive wave simulation where a string oscillates based on mouse clicks or drags:
- Implementation: Uses the wave equation with damping and stiffness terms, solved numerically (see wave_equation.ipynb).
- Features: Click or drag to perturb the string, visualized on an HTML canvas.
- Parameters:
  - c: Wave speed (0.01 m/s).
  - γ: Damping constant (200 s/m).
  - l: Stiffness term (0.002, dimensionless).
  - N: 200 points along the string.
- Interaction Modes:
  - DRAG_CENTER: Perturbs the string at the mouse position.
  - MOVE_LEFT_END: (Commented) Perturbs the left end of the string.-----------------------
#Wave Equation:
- Includes boundary conditions ((y(0, t) = y(L, t) = 0)) and discrete form for numerical solving.
- Describes coordinate conversion between string and canvas coordinates.
# How to Use
- View Presentation:
  - Download WAVES.pdf and open in a PDF viewer (e.g., Adobe Acrobat, Google Chrome).
- Run Simulation:
  - Clone the repository: git clone <repository-url>.
  - Open index.html in a web browser (e.g., Chrome, Firefox).
  - Click or drag on the canvas to perturb the wave and observe oscillations.
- Explore Wave Equation:
  - Open wave_equation.ipynb in Jupyter Notebook or JupyterLab to review the mathematical model.
- Modify Parameters:
  - Edit index.js to adjust c, γ, l, or N for different wave behaviors.
  - Ensure ( c \Delta t / \Delta x < 1 ) for numerical stability.
# Requirements
- Web browser for the simulation (no additional libraries needed).
- Jupyter Notebook or JupyterLab for viewing wave_equation.ipynb.
- Python 3.10+ (optional, for notebook exploration).
# Notes
- The simulation uses a canvas to render a red string on a black background, updated via requestAnimationFrame.
- The IPython notebook provides theoretical context but is not required to run the simulation.
- Images referenced in WAVES.pptx (e.g., image2.png) are not included; add them to the repository if needed.
- Ensure canvas size adjusts to window size (setSize function in index.js)..
# License
MIT License
