# 🚀 Rocket Simulator

A 2D rocket trajectory simulator with realistic physics, multi-stage support, and interactive visualization. Built for understanding rocket dynamics, experimenting with designs, and learning orbital mechanics fundamentals.

## 🎯 Project Overview

**Rocket Simulator** is a physics-accurate 2D simulation that models rocket flight from launch through orbit insertion. It implements proper rocket equations, atmospheric effects, and multi-stage mechanics in an accessible and interactive format.

**Key Features:**
- **Realistic Physics** - Proper rocket equation implementation with variable mass
- **Multi-Stage Rockets** - Support for complex staging sequences and optimization
- **Interactive Visualization** - Real-time 2D trajectory plotting and analysis
- **Rocket Designer** - Build and configure custom rockets with different engines and fuels
- **Mission Planning** - Optimize trajectories for specific orbital targets

## 🎯 Target Users

- **Students** learning rocket physics and orbital mechanics
- **Hobbyists** designing and testing model rocket concepts
- **Educators** teaching aerospace concepts with interactive simulations
- **Game Developers** needing realistic 2D rocket physics
- **Space Enthusiasts** wanting to understand how rockets actually work

## ✨ Features

### Physics Engine
- **2D Trajectory Simulation** - Accurate rocket motion in 2D space with proper physics
- **Rocket Equation** - Tsiolkovsky equation implementation with variable mass
- **Atmospheric Effects** - Air density, pressure, and drag modeling
- **Gravity Model** - Earth gravity with altitude variation
- **Multi-Stage Support** - Sequential stage separation and ignition

### Rocket Design
- **Custom Rocket Builder** - Configure rockets with different engines, fuel tanks, and payloads
- **Engine Database** - Real engine specifications (thrust, specific impulse, burn time)
- **Fuel Types** - Different propellant combinations with realistic properties
- **Mass Optimization** - Tools to optimize stage mass ratios and delta-v

### Visualization & Interface
- **Interactive 2D Plots** - Real-time trajectory visualization with matplotlib
- **Flight Parameters** - Live display of altitude, velocity, acceleration, and fuel remaining
- **Trajectory Analysis** - Apogee, perigee, orbital velocity, and efficiency calculations
- **Simple GUI** - User-friendly interface for rocket configuration and simulation control
- **Animation Mode** - Watch rockets fly in real-time with configurable speed

### Mission Planning
- **Target Orbits** - Set specific orbital targets (altitude, inclination)
- **Launch Optimization** - Find optimal launch angles and timing
- **Delta-V Calculations** - Precise delta-v requirements for mission planning
- **Staging Optimization** - Determine optimal staging points for maximum efficiency
- **Performance Analysis** - Compare different rocket configurations

### Data & Export
- **Flight Data Export** - Save trajectory data to CSV for analysis
- **Mission Reports** - Generate detailed reports with performance metrics
- **Rocket Configurations** - Save and load custom rocket designs
- **Batch Simulations** - Run multiple simulations with parameter variations

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/lguprojects/rocket-simulator.git
cd rocket-simulator

# Install dependencies
pip install -r requirements.txt

# Run a basic rocket simulation
python examples/simple_rocket.py

# Launch the interactive GUI
python rocket_simulator.py

# Try different rocket configurations
python examples/multi_stage_rocket.py
python examples/orbital_insertion.py
```

## 🛠️ Technology Stack

### Core Engine
- **Python 3.8+** - Primary development language for accessibility
- **NumPy** - Numerical computations and array operations
- **SciPy** - Scientific computing and optimization functions
- **Matplotlib** - 2D plotting, animation, and interactive visualization

### User Interface
- **Tkinter** - Built-in GUI framework for simple, cross-platform interface
- **Matplotlib GUI** - Interactive plots with zoom, pan, and data exploration
- **Jupyter Notebook** - Interactive development and analysis environment

### Data Management
- **JSON/YAML** - Configuration files and rocket specifications
- **CSV** - Data export for analysis in Excel or other tools
- **Pickle** - Saving and loading simulation states and rocket designs

### Optional Enhancements
- **PyQt5/6** - More advanced GUI features (if needed)
- **Pygame** - Enhanced animations and user interactions
- **Pandas** - Advanced data analysis capabilities

## 📁 Project Structure

```
rocket-simulator/
├── rocket_simulator.py      # Main GUI application
├── physics/                 # Core physics simulation
│   ├── __init__.py
│   ├── rocket_dynamics.py   # Rocket equation and motion
│   ├── atmosphere.py        # Atmospheric modeling
│   ├── integrator.py        # Numerical integration
│   └── utils.py             # Physics utilities
├── models/                  # Rocket and component models
│   ├── __init__.py
│   ├── rocket.py            # Rocket configuration class
│   ├── engines.py           # Engine database and models
│   ├── stages.py            # Multi-stage logic
│   └── propellants.py       # Fuel properties
├── visualization/           # Plotting and GUI
│   ├── __init__.py
│   ├── plots.py             # Matplotlib trajectory plots
│   ├── gui.py               # Tkinter interface
│   └── animation.py         # Real-time animation
├── mission/                 # Mission planning tools
│   ├── __init__.py
│   ├── optimizer.py         # Trajectory optimization
│   └── analysis.py          # Performance analysis
├── examples/                # Example simulations
│   ├── simple_rocket.py     # Basic single-stage rocket
│   ├── multi_stage_rocket.py # Multi-stage example
│   └── orbital_insertion.py # Orbit insertion demo
├── configs/                 # Configuration files
│   ├── engines.json         # Engine specifications
│   ├── rockets.json         # Pre-built rocket configs
│   └── settings.yaml        # Default simulation settings
├── tests/                   # Unit tests
│   ├── test_physics.py
│   ├── test_models.py
│   └── test_integration.py
├── docs/                    # Documentation
│   ├── user_guide.md
│   ├── physics_guide.md
│   └── api_reference.md
├── requirements.txt         # Python dependencies
└── README.md               # This file
```

## 🔧 Installation & Setup

### Prerequisites
- Python 3.8 or higher
- Standard Python libraries (tkinter usually included)
- 2GB+ RAM for typical simulations

### Dependencies Installation
```bash
# Install core dependencies
pip install numpy scipy matplotlib

# Install optional dependencies for enhanced features
pip install jupyter pandas pyyaml

# Or install all at once
pip install -r requirements.txt
```

### Verify Installation
```bash
# Run a quick test simulation
python examples/simple_rocket.py

# Launch the GUI to verify everything works
python rocket_simulator.py
```

## 🤝 Contributing

We welcome contributions from aerospace engineers, software developers, and simulation experts. Whether you're fixing bugs, optimizing performance, adding new features, or improving documentation.

### How to Contribute
1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/orbital-mechanics-enhancement`)
3. **Follow coding standards** - Ensure code quality and documentation
4. **Add comprehensive tests** - Unit tests, integration tests, and performance benchmarks
5. **Commit your changes** (`git commit -m 'Add orbital mechanics enhancement'`)
6. **Push to the branch** (`git push origin feature/orbital-mechanics-enhancement`)
7. **Open a Pull Request**

### Contributing Guidelines
- **Code Quality**: Follow PEP 8 for Python, include type hints
- **Performance**: Profile code for performance-critical sections
- **Documentation**: API documentation and technical implementation details
- **Testing**: Comprehensive test coverage including edge cases
- **Physics Accuracy**: Validate implementations against known solutions

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🌟 Acknowledgments

- NASA for excellent educational resources and public domain data
- The Kerbal Space Program community for inspiration and physics insights
- Scott Manley and other space YouTubers for making rocket science accessible
- Contributors to NumPy, SciPy, and matplotlib for excellent scientific libraries
- The open-source community for tools and educational resources

## 📞 Contact

- **Project Repository**: [https://github.com/lguprojects/Rocket-Simulator](https://github.com/lguprojects/Rocket-Simulator)
- **Issues**: Report bugs and request features via GitHub Issues
- **Discussions**: Questions, ideas, and physics discussions welcome
- **Wiki**: User guides, tutorials, and physics explanations

## 🗺️ Development Roadmap

### Phase 1: Core Physics (Month 1-2)
- [x] Project setup and basic structure
- [ ] 2D rocket dynamics with proper physics
- [ ] Rocket equation implementation (Tsiolkovsky)
- [ ] Basic atmospheric drag modeling
- [ ] Simple gravity model with altitude variation

### Phase 2: Multi-Stage Support (Month 3-4)
- [ ] Multi-stage rocket configuration
- [ ] Stage separation and ignition logic
- [ ] Fuel consumption and mass tracking
- [ ] Basic trajectory optimization
- [ ] Engine database with real specifications

### Phase 3: Visualization & Interface (Month 5-6)
- [ ] Interactive matplotlib trajectory plots
- [ ] Real-time flight parameter display
- [ ] Simple GUI with tkinter
- [ ] Animation mode for flight visualization
- [ ] Configuration file system for rockets

### Phase 4: Mission Planning (Month 7-8)
- [ ] Target orbit specification
- [ ] Launch angle optimization
- [ ] Delta-v calculations and analysis
- [ ] Performance comparison tools
- [ ] Mission report generation

### Phase 5: Polish & Features (Month 9-12)
- [ ] Enhanced GUI with better controls
- [ ] Batch simulation capabilities
- [ ] Data export and analysis tools
- [ ] Example missions and tutorials
- [ ] Comprehensive documentation

### Future Enhancements
- [ ] 3D visualization (pygame or simple OpenGL)
- [ ] More complex atmospheric models
- [ ] Wind effects and turbulence
- [ ] Orbital perturbation effects
- [ ] Historical mission recreation

---

**Learn rocket physics through interactive simulation and experimentation.**

Built for curiosity, education, and the joy of understanding how rockets work! 🚀 
