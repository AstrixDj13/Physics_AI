# Physics_AI
This code implements a **Physics-Informed Neural Network (PINN) using a Transformer architecture** to solve the **1D heat equation**. The heat equation is discretized using **finite differences**, and a **Gaussian initial condition** is imposed. The solution is computed using **solve_ivp** for ground truth. The **Transformer-based PINN** is trained with **finite-difference approximations for derivatives** instead of autograd, enforcing both the **PDE residual loss** and the **initial condition loss**. The model is trained using **Adam optimizer** on GPU, and predictions are generated over the full space-time domain. The final results compare the **true solution vs. PINN-predicted solution** using heatmaps and sequential time-marching predictions. This approach demonstrates the feasibility of using deep learning to approximate **PDE solutions efficiently without explicit numerical solvers**.

![image](https://github.com/user-attachments/assets/ec4daaad-2f92-448b-b01c-1342737b1534)

![image](https://github.com/user-attachments/assets/8815889f-16db-4d7a-9f92-2d9cd95f3c36)


