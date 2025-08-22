

Built-in Diagnostics and Validation
To ensure the robustness and physical validity of the simulations, a suite of diagnostic tools is integrated directly into the workflow. These tools perform critical checks on the model setup and results:

    Driving Stress Analysis: A function (analyse_driving_stress) calculates and compares the driving stress at the domain boundaries to verify that the periodic setup is correctly balanced and not introducing artificial stress gradients.

    Friction and Boundary Conditions: Dedicated debugging functions (debug_friction_setup, diagnose_boundary_conditions) validate the implementation of the basal friction laws and check for inconsistencies in the boundary condition application.

    Mesh Quality: A visual mesh check (visual_mesh_check) allows for the inspection of the generated mesh to confirm that the adaptive refinement is performing as expected.

