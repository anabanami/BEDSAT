
### pre-empting questions from the panel.

2. Methodology & Theoretical Framework

  * You plan to use NVIDIA's PhysicsNeMo framework. What specific governing equations (PDEs) will you enforce as physical constraints, and how do you believe this will improve upon a purely data-driven machine learning approach?

  * Your results clearly show that non-linear rheology ($n=4$) produces substantially different surface expressions compared to linear rheology ($n=1$). Given this, why do you think modern methods like Ockenden et al. (2023) still rely on a linear rheology assumption? What trade-offs are they making?

  * You propose to develop a new bed topography for the *entire* Antarctic continent. What are the computational requirements for this, particularly for training a Physics-ML model at this scale? Do you have the necessary resources allocated?

  * In your plan to address aeolian noise, you propose adding a "statistically realistic aeolian roughness layer" to your synthetic training data. How will you validate that this synthetic noise accurately represents the real-world processes and spatial patterns described by Poizat et al. (2024)?

3. Progress & Results So Far

  * Your grid convergence analysis for Scenario S2 (frozen bed, non-linear rheology) shows a very large sensitivity to vertical resolution, where low-resolution runs converge to a much slower velocity ($\\approx11\~m/a$) than high-resolution runs ($\\approx37\~m/a$). Can you provide a physical explanation for why the model is so sensitive in this specific scenario?

  * Your phase analysis finds a phase shift of approximately $2\\pi/3$ for an isolated Gaussian bump, which differs from Budd's periodic theory. What are the practical implications of this finding for your BedSAT inversion framework when it encounters the complex, non-periodic topography of the real world?

  * What was the most unexpected challenge you faced when replicating the ISMIP-HOM experiments, and what key lesson did you learn about the ISSM that you will carry forward?

4. Future Work & Timeline

  * Your timeline shows you plan to "Obtain ML training data" from roughly July to December 2025. Can you estimate how many synthetic ISSM simulations this requires and the total computation time? Does your timeline account for this?

  * Objective 2, developing the continent-wide topography dataset, is a major undertaking scheduled to start in mid-2026. What are the key decision points or milestones between now and then that must be met to ensure this phase is successful?

  * You have selected the Aurora Subglacial Basin as a validation site. Why is this region particularly well-suited for testing and validating the BedSAT framework?

5. Limitations & Contingency Planning

  * You list "computational cost" as a potential limitation. If the Physics-ML approach proves too computationally intensive for a continental-scale inversion, what is your backup plan? Would you restrict the scope to a few key Antarctic catchments?
  
  * What if, in some regions, the aeolian signal is so dominant that no reliable bed signal can be inverted for, even with your advanced method? How will your final BedSAT dataset represent or flag these areas of extremely high uncertainty?

