# Continuous Variable Co-location Mining Framework

This repository provides a comprehensive framework for Continuous Variable Co-location Mining, including tools for influence density calculation, co-location analysis, and statistical validation. The implementation is designed to handle both binary and ternary co-location patterns using a well-defined workflow.

---

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
   - [Utilities](#utilities)
   - [Analysis Workflow](#analysis-workflow)
5. [Contributing](#contributing)
6. [License](#license)

---

## Overview
This framework enables:
- **Influence density calculation** using Gaussian Kernel Density Estimation (KDE).
- **Co-location analysis** for both binary and ternary patterns.
- **Visualization** of spatial patterns and statistical relationships.
- **Statistical validation** using permutation tests.

The framework is particularly useful for identifying spatial interactions and validating spatial hypotheses in diverse datasets.

---

## Features
- **Generate Sample Points:** Automatically create a spatial grid based on the dataset's bounding box.
- **Influence Calculation:** Compute spatial influence densities using KDE.
- **Co-location Analysis:** Analyze binary and ternary spatial interactions.
- **Visualization Tools:** Visualize influence densities and co-location results.
- **Permutation Testing:** Validate statistical significance of patterns.

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Collocation-Mining-Project.git
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   
## Usage

### Utilities
The repository includes utility functions to preprocess data and perform core calculations:

- **`calculate_pvalues`**: Calculates p-values for pairwise correlations.
- **`mean_std`**: Computes the mean and standard deviation of data.
- **`ProcessData`**: Preprocesses spatial datasets.
- **`generate_sample_points`**: Generates a grid of sample points for spatial analysis.

---

### Analysis Workflow
Follow these steps to conduct a complete analysis:

1. **Read Data**: Load and preprocess the dataset.
2. **Generate Sample Points**: Create a grid using `generate_sample_points`.
3. **Calculate Influence Functions**:
   - Use `influence` or `influenceO` for influence density calculation.
4. **Visualize Influence**: Generate heatmaps or contour plots.
5. **Co-location Analysis**:
   - Use `equationC3NoLog` for ternary co-location.
   - Use `equationC2NoLog` for binary co-location.
6. **Visualization of Co-locations**: Plot the co-location results.
7. **Permutation Test**: Perform statistical validation for binary co-location results.
8. **Save Results**: Export co-location and permutation test results.

---

## Contributing
Contributions are welcome! If you'd like to contribute:

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
3. Commit your changes:
 ```bash
 git commit -m "Add feature description"
```
4. Push the branch and create a pull request.

## License
This project is licensed under the [MIT License](LICENSE).

---

## Contact
For questions or collaboration, please reach out to [your-email@example.com](mailto:mdmahin3@gmail.com).
