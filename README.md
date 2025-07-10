# Neural ODEs for Chemical Kinetics Simulations

### 🎯 Goal
You are provided with both training and testing time-series datasets for a chemical reaction. These datasets record the temporal evolution of chemical species and 
temperature, similar to the systems analyzed in the ChemNode research paper. The testing dataset represents a chemical reaction with a different initial condition 
to that of training data. <br>  
**Note**: While the ChemNode paper focuses on hydrogen combustion, your assignment uses 
the GRI v3.0 mechanism, which models methane combustion. The underlying modeling 
approaches and analysis remain similar, but the reaction mechanism is different. 

### 🚀 Approach
- Done an analysis on the provided training dataset. Based on the variation and correlation of chemical species wrt to temperature, I selected the top 6 species involved in
the chemical reaction. The mapping of the species (y1 to y53) was done from the official documentation available on the internet.

<img width="541" height="341" alt="Image" src="https://github.com/user-attachments/assets/e0398a8c-ae60-4116-a78e-de791cd55163" />

- Trained an Neural ODE utilizing pytorch 'torchdiffeq' library. We used an adaptive step solver ‘dopri5’ (Runge-Kutta of order 5 of 
Dormand-Prince-Shampine).


### 📢 Future Work
For Scientific ML, coding is usually done using Julia programming language, which offers better mathematical operations and visualizations for simulation type of problems.


