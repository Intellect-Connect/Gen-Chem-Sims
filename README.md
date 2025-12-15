# Gen-Chem-Sims
Interactive general chemistry simulations and visualizations covering atomic structure, chemical bonding, thermodynamics, and foundational concepts. Perfect for introductory chemistry students and educators.

# Gen Chem Sims ⚗️🔬

> Interactive simulations and visualizations for general chemistry concepts, from atomic structure to thermodynamics

[![License](https://img.shields.io/badge/license-All%20Rights%20Reserved-red.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/CHEM103-ckeenan/Gen-Chem-Sims.svg)](https://github.com/CHEM103-ckeenan/Gen-Chem-Sims/stargazers)
[![GitHub Issues](https://img.shields.io/github/issues/CHEM103-ckeenan/Gen-Chem-Sims.svg)](https://github.com/CHEM103-ckeenan/Gen-Chem-Sims/issues)

---

## 📖 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Screenshots](#screenshots)
- [Installation](#installation)
- [Usage](#usage)
- [Topics Covered](#topics-covered)
- [Roadmap](#roadmap)
- [Technology Stack](#technology-stack)
- [Contributing](#contributing)
- [Educational Standards](#educational-standards)
- [FAQ](#faq)
- [License](#license)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

---

## 📖 Overview

**Gen Chem Sims** is a comprehensive collection of interactive simulations designed to visualize and teach fundamental general chemistry concepts. Whether you're a student struggling with abstract chemical principles, an educator looking to enhance your lectures, or a self-learner exploring chemistry, these simulations bring chemical phenomena to life through dynamic, interactive visualizations.

### Why Gen Chem Sims?

Chemistry is inherently visual, yet textbooks and lectures often present concepts in static, abstract ways. Gen Chem Sims bridges this gap by:

- **Making the Invisible Visible**: See atoms, molecules, and electrons in motion
- **Interactive Learning**: Manipulate variables and observe real-time changes
- **Immediate Feedback**: Understand cause-and-effect relationships instantly
- **Self-Paced Exploration**: Learn at your own speed without pressure
- **Accurate Representations**: Scientifically accurate models and simulations

---

## ✨ Features

### 🔬 Interactive Simulations

- **Real-time manipulation** of variables (temperature, pressure, concentration)
- **Step-by-step animations** of chemical processes
- **Visual feedback** for understanding cause and effect
- **Pause, rewind, and replay** functionality

### 📊 Visual Tools

- **3D molecular viewers** with rotation and zoom
- **Interactive periodic table** with element properties
- **Dynamic graphs** showing relationships between variables
- **Color-coded visualizations** for clarity

### 🎓 Educational Features

- **Guided tutorials** for each simulation
- **Practice problems** with instant feedback
- **Conceptual questions** to test understanding
- **Reference materials** and explanations
- **Progress tracking** (coming soon)

### 🌐 Accessibility

- **Web-based** - works in any modern browser
- **Mobile-friendly** responsive design
- **No installation** required for basic use
- **Offline mode** available for downloaded version

---

## 📸 Screenshots

### Atomic Structure Visualization
![Atomic Structure](docs/images/atomic-structure-demo.png)
*Interactive 3D visualization of electron orbitals and probability distributions*

### Gas Laws Simulator
![Gas Laws](docs/images/gas-laws-demo.png)
*Real-time manipulation of pressure, volume, and temperature with PV=nRT calculations*

### Titration Curve Generator
![Titration](docs/images/titration-demo.png)
*Dynamic pH curves with equivalence point indicators*

---

## 🚀 Installation

### Option 1: Web Version (Recommended for Most Users)

Simply visit: **[Your hosted URL here]**

No installation required! Works in Chrome, Firefox, Safari, and Edge.

### Option 2: Local Installation

#### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- Modern web browser

#### Steps
```bash
# Clone the repository
git clone https://github.com/CHEM103-ckeenan/Gen-Chem-Sims.git

# Navigate to directory
cd Gen-Chem-Sims

# Install dependencies
npm install

# Run development server
npm start

# Open browser to localhost:3000
```

### Option 3: Download Desktop App

Download the standalone application for offline use:
- [Windows Installer](releases/windows)
- [macOS App](releases/macos)
- [Linux AppImage](releases/linux)

---

## 💻 Usage

### Getting Started

1. **Choose a Topic**: Select from the main menu or use the search function
2. **Read the Overview**: Each simulation includes background information
3. **Interact**: Adjust sliders, input values, or click interactive elements
4. **Observe**: Watch the visualization respond in real-time
5. **Test**: Try practice problems to reinforce learning

### Example: Gas Laws Simulation
```javascript
// Access the simulation programmatically (for educators creating custom exercises)
const gasSimulation = new GasLawSimulator({
  initialPressure: 1.0,  // atm
  initialVolume: 22.4,   // L
  initialTemp: 273,      // K
  gasType: 'ideal'
});

// Change conditions
gasSimulation.setTemperature(373); // Heat to 100°C
console.log(gasSimulation.getPressure()); // See new pressure

// Visualize
gasSimulation.render('canvas-id');
```

### Keyboard Shortcuts

- `Space` - Pause/Play animation
- `R` - Reset simulation
- `H` - Show help overlay
- `F` - Fullscreen mode
- `←/→` - Previous/Next step (in step-by-step mode)

---

## 📚 Topics Covered

### Unit 1: Atomic Structure & Periodicity ⚛️

#### 1.1 Atomic Models
- Bohr model visualization
- Quantum mechanical model
- Electron probability distributions
- Orbital shapes (s, p, d, f)

#### 1.2 Electron Configuration
- Aufbau principle simulator
- Orbital filling diagrams
- Noble gas notation
- Valence electrons identifier

#### 1.3 Periodic Trends
- Interactive periodic table
- Atomic radius trends
- Ionization energy graphs
- Electronegativity visualization
- Electron affinity comparison

**Simulations:**
- `atomic-orbitals-3d.html` - 3D visualization of atomic orbitals
- `electron-config.html` - Build electron configurations
- `periodic-trends.html` - Explore periodic table trends

---

### Unit 2: Chemical Bonding 🔗

#### 2.1 Ionic Bonding
- Electron transfer animations
- Crystal lattice structures
- Lattice energy calculations
- Ionic compound formation

#### 2.2 Covalent Bonding
- Lewis structure builder
- VSEPR geometry predictor
- Bond polarity calculator
- Resonance structure drawer

#### 2.3 Metallic Bonding
- Electron sea model
- Metallic properties simulator
- Alloy composition explorer

#### 2.4 Intermolecular Forces
- Hydrogen bonding visualizer
- Dipole-dipole interactions
- London dispersion forces
- Strength comparisons

**Simulations:**
- `lewis-structures.html` - Draw and validate Lewis structures
- `molecular-geometry.html` - VSEPR theory and 3D shapes
- `polarity-simulator.html` - Determine molecular polarity
- `intermolecular-forces.html` - Compare IMF strengths

---

### Unit 3: States of Matter 🌡️

#### 3.1 Kinetic Molecular Theory
- Gas particle motion simulator
- Temperature effect on speed
- Pressure from collisions
- Distribution of speeds

#### 3.2 Phase Changes
- Heating/cooling curves
- Phase diagram explorer
- Energy changes (ΔH)
- Critical point visualization

#### 3.3 Gas Laws
- Boyle's Law (P-V relationship)
- Charles's Law (V-T relationship)
- Gay-Lussac's Law (P-T relationship)
- Combined Gas Law
- Ideal Gas Law (PV=nRT)
- Real gases vs. ideal gases

**Simulations:**
- `kinetic-theory.html` - Visualize gas particle motion
- `phase-diagram.html` - Interactive phase diagrams
- `gas-laws-combo.html` - All gas laws in one simulation
- `ideal-vs-real.html` - Compare ideal and real gas behavior

---

### Unit 4: Chemical Reactions ⚗️

#### 4.1 Reaction Types
- Synthesis reactions
- Decomposition reactions
- Single displacement
- Double displacement
- Combustion reactions

#### 4.2 Stoichiometry
- Balancing equations tool
- Mole-to-mole conversions
- Mass-to-mass calculations
- Limiting reagent identifier
- Percent yield calculator

#### 4.3 Solutions
- Molarity calculator
- Dilution simulator
- Solubility curves
- Precipitation reactions

**Simulations:**
- `equation-balancer.html` - Balance chemical equations
- `stoichiometry-calc.html` - Stoichiometric calculations
- `limiting-reagent.html` - Identify limiting reagents
- `molarity-dilution.html` - Solution preparation

---

### Unit 5: Thermodynamics & Kinetics 🔥

#### 5.1 Thermochemistry
- Exothermic vs. endothermic
- Enthalpy diagrams
- Hess's Law calculator
- Calorimetry simulator
- Bond energy calculations

#### 5.2 Chemical Kinetics
- Reaction rate graphs
- Concentration vs. time
- Rate law determinations
- Collision theory animator
- Activation energy diagrams
- Catalyst effects

#### 5.3 Reaction Mechanisms
- Elementary steps
- Rate-determining step
- Reaction coordinate diagrams
- Transition states

**Simulations:**
- `enthalpy-diagrams.html` - Energy diagrams for reactions
- `calorimetry.html` - Virtual calorimeter
- `reaction-rates.html` - Rate vs. concentration graphs
- `activation-energy.html` - Effect of temperature and catalysts
- `collision-theory.html` - Molecular collision animations

---

### Unit 6: Chemical Equilibrium ⚖️

#### 6.1 Dynamic Equilibrium
- Reversible reactions
- Equilibrium constant (Keq)
- Reaction quotient (Q)
- Le Chatelier's principle
- Effect of stress on equilibrium

#### 6.2 Acid-Base Equilibrium
- Strong vs. weak acids/bases
- pH calculations
- Ka and Kb calculations
- Titration curve generator
- Buffer solutions
- Indicators and pH ranges

#### 6.3 Solubility Equilibrium
- Ksp calculations
- Common ion effect
- Precipitation predictions
- Complex ion formation

**Simulations:**
- `equilibrium-sim.html` - Dynamic equilibrium visualization
- `le-chatelier.html` - Apply stress to systems
- `ph-calculator.html` - Calculate pH for various solutions
- `titration-curves.html` - Generate and analyze titration curves
- `buffer-capacity.html` - Test buffer effectiveness
- `solubility-ksp.html` - Solubility product calculations

---

### Unit 7: Electrochemistry 🔋

#### 7.1 Oxidation-Reduction
- Oxidation number calculator
- Balancing redox equations
- Half-reaction method
- Oxidizing/reducing agents

#### 7.2 Electrochemical Cells
- Galvanic cell builder
- Electrolytic cell simulator
- Standard reduction potentials
- Nernst equation calculator
- Battery voltage predictor

#### 7.3 Applications
- Corrosion prevention
- Electroplating simulator
- Fuel cells
- Battery technology

**Simulations:**
- `redox-balancer.html` - Balance redox equations
- `galvanic-cell.html` - Build and test galvanic cells
- `electrolysis.html` - Electrolytic cell simulator
- `nernst-calculator.html` - Calculate cell potentials

---

## 🗺️ Roadmap

### Version 1.0 (Current)
- ✅ Core simulations for all major topics
- ✅ Interactive periodic table
- ✅ Basic stoichiometry tools
- ✅ Gas law simulations

### Version 1.5 (In Progress)
- 🔄 Enhanced 3D molecular viewer
- 🔄 Practice problem sets with solutions
- 🔄 User progress tracking
- 🔄 Mobile app optimization

### Version 2.0 (Planned)
- 📋 Virtual laboratory experiments
- 📋 AI-powered homework helper
- 📋 Collaborative learning features
- 📋 Integration with LMS platforms (Canvas, Blackboard)
- 📋 Augmented reality molecular viewer

### Future Enhancements
- Multi-language support
- Accessibility improvements (screen readers, high contrast)
- Gamification elements (achievements, leaderboards)
- Teacher dashboard for class management
- Custom simulation builder

---

## 🛠️ Technology Stack

### Frontend
- **React.js** - UI framework
- **Three.js** - 3D visualizations
- **D3.js** - Data visualization and graphs
- **Tailwind CSS** - Styling
- **Framer Motion** - Animations

### Backend
- **Node.js** - Server runtime
- **Express.js** - API framework
- **MongoDB** - Database (for user progress)

### Scientific Libraries
- **RDKit.js** - Chemical structure handling
- **Math.js** - Mathematical calculations
- **ChemDoodle** - 2D chemical structure drawing

### Build Tools
- **Vite** - Build tool and dev server
- **TypeScript** - Type safety
- **Jest** - Testing framework

---

## 🤝 Contributing

We welcome contributions from the chemistry education community! Whether you're a developer, educator, or student, there are many ways to help.

### Ways to Contribute

1. **Report Bugs**: Found an error? [Open an issue](https://github.com/CHEM103-ckeenan/Gen-Chem-Sims/issues)
2. **Suggest Features**: Have an idea? [Start a discussion](https://github.com/CHEM103-ckeenan/Gen-Chem-Sims/discussions)
3. **Improve Documentation**: Fix typos, clarify explanations
4. **Add Content**: Create new simulations or practice problems
5. **Code Contributions**: Fix bugs or implement features

### Contribution Guidelines

Please read our [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines on:
- Code style and standards
- Pull request process
- Testing requirements
- Documentation expectations

### Getting Help

- 💬 [Discussions](https://github.com/CHEM103-ckeenan/Gen-Chem-Sims/discussions) - Ask questions and share ideas
- 🐛 [Issues](https://github.com/CHEM103-ckeenan/Gen-Chem-Sims/issues) - Report bugs and request features
- 📧 Email: [your-email@example.com]

---

## 🎓 Educational Standards

Gen Chem Sims aligns with major educational standards and curricula:

### AP Chemistry
- Covers all 9 units of the AP Chemistry curriculum
- Practice problems mirror AP-style questions
- Conceptual understanding emphasized

### American Chemical Society (ACS) Guidelines
- Meets ACS General Chemistry guidelines
- Appropriate depth for first-year college chemistry

### Next Generation Science Standards (NGSS)
- HS-PS1: Matter and Its Interactions
- HS-PS3: Energy
- Science and Engineering Practices

### Common Core State Standards
- Mathematical Practice Standards
- Integration of mathematics and science

---

## ❓ FAQ

### General Questions

**Q: Is Gen Chem Sims free to use?**  
A: The web version is currently available for evaluation. For licensing information for educational institutions or commercial use, please contact us.

**Q: Do I need to create an account?**  
A: Not for basic use! Account creation is optional and only needed for saving progress.

**Q: What browsers are supported?**  
A: Chrome, Firefox, Safari, and Edge (latest versions). Mobile browsers also supported.

**Q: Can I use this offline?**  
A: Yes! Download the desktop application for full offline access.

### For Students

**Q: Will this help me pass my chemistry exam?**  
A: While Gen Chem Sims is a powerful learning tool, it's designed to supplement your coursework, not replace it. Use it alongside your textbook, lectures, and practice problems.

**Q: Are the answers provided?**  
A: Yes! Practice problems include step-by-step solutions.

**Q: Can I share my progress with my teacher?**  
A: Progress sharing features are coming in Version 1.5.

### For Educators

**Q: Can I use this in my classroom?**  
A: For individual educator use in a classroom setting, please contact us for licensing. We offer discounted rates for educational institutions.

**Q: Can I create custom simulations?**  
A: The custom simulation builder is planned for Version 2.0. Currently, you can request specific simulations by opening an issue.

**Q: Is there a teacher dashboard?**  
A: Coming in Version 2.0! It will include class management and progress tracking.

**Q: Can I embed simulations in my LMS?**  
A: Not yet, but LMS integration is planned for Version 2.0.

### Technical Questions

**Q: My simulation isn't loading. What should I do?**  
A: Try refreshing the page, clearing your browser cache, or using a different browser. If problems persist, [open an issue](https://github.com/CHEM103-ckeenan/Gen-Chem-Sims/issues).

**Q: Can I run this on a Raspberry Pi or low-spec computer?**  
A: Most simulations will work, but 3D visualizations may be slower. Try the "Performance Mode" in settings.

**Q: Is my data private?**  
A: Yes! We don't collect or store personal information without your explicit consent. See our [Privacy Policy](PRIVACY.md).

---

## 📄 License & Usage

**© [Your Name] 2025. All Rights Reserved.**

This software is proprietary and confidential. Unauthorized copying, distribution, or use of this software, via any medium, is strictly prohibited.

### Licensing Options

For licensing inquiries, please contact:

- **Individual Educators**: Classroom use licenses available
- **Educational Institutions**: Site licenses with volume discounts
- **Commercial Use**: Custom licensing available
- **Open Source Projects**: Special consideration on request

📧 Email: [your-email@example.com]  
🌐 Website: [your-website.com]

---

## 📧 Contact

### Maintainer
**[Your Name]**  
Chemistry Educator & Developer  
📧 [your-email@example.com]  
🌐 [your-website.com]  
🐦 [@yourtwitter](https://twitter.com/yourtwitter)

### Support
- 🐛 Bug Reports: [GitHub Issues](https://github.com/CHEM103-ckeenan/Gen-Chem-Sims/issues)
- 💡 Feature Requests: [GitHub Discussions](https://github.com/CHEM103-ckeenan/Gen-Chem-Sims/discussions)
- 📧 General Inquiries: [your-email@example.com]

---

## 🙏 Acknowledgments

### Inspiration & Resources
- Chemistry education community on Reddit and Discord
- PhET Interactive Simulations (University of Colorado Boulder)
- ChemCollective (Carnegie Mellon University)
- POGIL (Process Oriented Guided Inquiry Learning) methodology

### Special Thanks
- Beta testers and early adopters
- Students who provided feedback
- Fellow chemistry educators for suggestions
- Open source community for amazing tools

### Built With
- [React](https://reactjs.org/)
- [Three.js](https://threejs.org/)
- [D3.js](https://d3js.org/)
- [RDKit.js](https://github.com/rdkit/rdkit-js)
- And many other amazing open source projects

---

## 📊 Project Stats

![GitHub repo size](https://img.shields.io/github/repo-size/Intellect-Connect-ckeenan/Gen-Chem-Sims)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/Intellect-Connect-ckeenan/Gen-Chem-Sims)
![GitHub last commit](https://img.shields.io/github/last-commit/Intellect-Connect-ckeenan/Gen-Chem-Sims)

---

## 🌟 Star History

If you find Gen Chem Sims helpful, please consider giving it a star! ⭐

[![Star History Chart](https://api.star-history.com/svg?repos=CHEM103-ckeenan/Gen-Chem-Sims&type=Date)](https://star-history.com/#Intellect-Connect-ckeenan/Gen-Chem-Sims&Date)

---

<div align="center">

**Made with ❤️ and ☕ for chemistry students everywhere**

[⬆ Back to Top](#gen-chem-sims-️)

</div>
