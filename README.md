# Root Finding Algorithms Visualizer

## Project Description and Purpose

The Root Finding Algorithms Visualizer is an interactive front-end web application designed to help users understand and explore the behavior of classical numerical root-finding methods. It allows users to input a mathematical function and visually observe how different algorithms iteratively converge toward a root.

The project is intended for educational use in numerical analysis, engineering, computer science, and applied mathematics. It bridges theoretical concepts with intuitive visual feedback, making abstract iterative processes easier to comprehend.

## Features and Functionality

- Interactive input for mathematical functions of one variable.
- Support for multiple root-finding algorithms:
  - Bisection Method
  - Newton-Raphson Method
  - Secant Method
  - Regula Falsi (False Position) Method
- Real-time graph visualization of the function f(x).
- Step-by-step and animated execution of algorithms.
- Adjustable animation speed.
- Convergence control using tolerance and maximum iteration limits.
- Iteration log displaying:
  - Iteration number
  - Current root estimate
  - Function value at the estimate
  - Error estimate
  - Method-specific notes
- Visual indicators for:
  - Current root estimate
  - Search intervals
  - Secant and tangent approximations where applicable
- Built-in documentation modal explaining theory and usage.

## Requirements Summary

Based on the project requirements specification:

- The system must provide a user-friendly graphical interface for function input and algorithm selection.
- Multiple root-finding algorithms must be supported, including Bisection, Newton-Raphson, Secant, and Regula Falsi.
- Users must be able to define initial guesses or intervals depending on the chosen method.
- The convergence process must be visualized iteratively on a graph.
- Convergence criteria must include tolerance thresholds and maximum iteration limits.
- Error estimation must be calculated and displayed for each iteration.
- Users must be able to control execution speed and step through iterations.
- The final root and iteration summary must be presented clearly.
- Documentation and theoretical explanations must be included within the project.
- The design should allow future extensibility for additional algorithms.

## Project Structure Overview
 ├── index.html        # Complete application including HTML, CSS, and JavaScript

 ├── RootFindingAlgorithmsVisualizer.pdf   # Project requirements and specification


The project is implemented as a single self-contained HTML file with embedded styles and scripts. No external libraries or build tools are required.

## Setup and Installation Instructions

This project does not require installation or a build process.

1. Download or clone the repository.
2. Ensure that `index.html` is present in the project root.
3. Open `index.html` in any modern web browser such as Chrome, Firefox, or Edge.

No server, package manager, or additional dependencies are required.

## Usage Instructions

1. Open the application in a web browser.
2. Enter a mathematical function in the function input field.
   - Supported operators: `+`, `-`, `*`, `/`, `^`
   - Supported functions: `sin`, `cos`, `tan`, `exp`, `log`, `sqrt`
3. Select a root-finding algorithm from the dropdown menu.
4. Provide the required initial parameters:
   - Interval `[a, b]` for Bisection and Regula Falsi
   - Initial guess `x0` for Newton-Raphson
   - Two initial points `x0` and `x1` for Secant
5. Set the tolerance and maximum number of iterations.
6. Click **Set/Reset** to initialize the visualization.
7. Use:
   - **Step** to advance one iteration at a time
   - **Play** to run the animation automatically
   - **Pause** to stop the animation
8. Review the iteration log and final result displayed below the graph.

## Assumptions and Limitations

- The function parser evaluates user input using JavaScript expressions and does not perform symbolic validation.
- Newton-Raphson uses numerical differentiation, which may be unstable near points where the derivative is close to zero.
- Visualization ranges are automatically determined based on initial parameters and may not capture extreme function behavior.
- The application is intended for educational visualization and not for high-precision numerical computation.

## Technologies Used

- HTML5
- CSS3
- Vanilla JavaScript
- HTML Canvas API

No external frameworks or libraries are used.

## Future Improvements

Potential enhancements inferred from the requirements include:

- Adding more root-finding algorithms such as Fixed Point Iteration or Brent’s Method.
- Side-by-side comparison of multiple algorithms on the same function.
- Enhanced error analysis charts showing convergence rates.
- Exporting iteration data for further analysis.
- Modularizing JavaScript code for improved maintainability and extensibility.

## License

License information is not specified. A suitable open-source license can be added as needed.
