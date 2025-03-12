# SPDFEM: Simulation of Photonic Devices using Finite Element Method

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![FEniCS](https://img.shields.io/badge/powered%20by-FEniCS-blue.svg)](https://fenicsproject.org/)

SPDFEM is a powerful Python package for simulating and analyzing photonic devices using the Finite Element Method. It provides a robust framework for modeling electromagnetic wave propagation, light-matter interactions, and optical phenomena in complex photonic structures.

## 🚀 Features

- Full electromagnetic field simulation using FEM
- Support for complex geometries and material properties
- Built-in mesh generation and handling
- Visualization tools for field distributions
- Comprehensive validation and verification framework
- Easy-to-use interface for defining simulation parameters
- Extensive documentation and tutorials

## 📋 Prerequisites

- Linux Operating System
- Python 3.7 or higher
- FEniCS 2019.1.0
- Additional Python packages:
  ```
  matplotlib
  numpy
  scipy
  pytest (for running tests)
  ```

## 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/SPDFEM.git
   cd SPDFEM
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## 🎯 Quick Start

1. Navigate to the `src` directory:
   ```bash
   cd src
   ```

2. Run the main simulation:
   ```bash
   python main.py
   ```

3. Follow the interactive prompts to:
   - Specify input file path (e.g., `Input/Input_t1.txt`)
   - Provide mesh file path (e.g., `Mesh/G_fill_t1.xml`)
   - Define physical regions file (e.g., `Mesh/G_fill_pr_t1.xml`)
   - Set facet regions file (e.g., `Mesh/G_fill_fc_t1.xml`)

4. Results will be saved in the `FEM Output` directory as `.pvd` and `.vtk` files.

## 📚 Documentation

- [Problem Statement](docs/ProblemStatement/ProblemStatement.pdf) - Detailed explanation of the physical problem
- [System Requirements Specification](docs/SRS/SRS.pdf) - Technical requirements and theoretical background
- [Validation & Verification Plan](docs/VnVPlan/VnVPlan.pdf) - Testing methodology
- [V&V Report](docs/VnV%20Report/VnV%20Report.pdf) - Validation results and analysis
- [Design Documentation](docs/Design) - Software architecture and modular design
- [Tutorial Notebook](src/SPDFM%20Tutorial%20.ipynb) - Step-by-step guide for beginners

## 🧪 Testing

Run the test suite using pytest:
```bash
pytest src/test_*.py
```

Key test files:
- `test_constparam.py`: Validates constant parameters
- `test_inputparam.py`: Tests input parameter handling
- `test_visual_ls.py`: Verifies visualization functions
- `test_meshinput.py`: Ensures proper mesh handling

## 📁 Project Structure

```
SPDFEM/
├── src/                 # Source code
│   ├── main.py         # Main simulation entry point
│   ├── fem_solver.py   # FEM implementation
│   ├── inputparam.py   # Parameter handling
│   └── ...
├── docs/               # Documentation
├── Mesh/              # Example mesh files
├── Input/             # Input configuration files
└── FEM Output/        # Simulation results
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

For questions, issues, or collaboration opportunities, please [open an issue](https://github.com/yourusername/SPDFEM/issues) or contact the repository maintainers.

---

Happy simulating with SPDFEM! 🌟
