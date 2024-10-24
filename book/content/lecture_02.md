# Lecture 2

The previous lecture introduced Operations Research as a scientific approach to optimal decision-making. In this lecture, we shall lay down the foundations of this scientific approach.

---

## The Five Step Process of Operations Research

### 1. Define the Problem

  Most problems are initially described vaguely, and therefore our first task is to precisely articulate the problem by identifying the:
  - **Objective** – Determine the goal such as resource minimization, service maximization, cost minimization, profit maximization, etc.
  - **Decisions** – Determine the key choices that need to be made, such as how much to procure, where to allocate resources, which route to select, etc.
  - **Constraints** – Determine limitations on the decisions, such as budgetary limits, resource availability, regulatory requirements, operational capacities, etc.
   
  Through thorough consultations, identify how all relevant stakeholders, such as owners, employees, suppliers, customers, and government influence the goal, choices, and limitations.
  
  For instance, consider a highway operations management firm maintaining the Chennai-Bangalore Expressway. The firm seeks to maximize toll revenue collected from private and commercial vehicles using the expressway; however, it must adhere to toll price regulations (maximum/minimum toll price) set by the National Highway Authority of India (NHAI) to facilitate sufficient traffic flow and tax collection.

  - **Objective** – Revenue maximization
  - **Decisions** – A toll price for private vehicles and another for commercial vehicles
  - **Constraints** – Maximum/minimum toll price for private vehicles and commercial vehicles, as regulated by NHAI.

### 2. Collect Relevant Data

  Once the problem’s objective function, decision variables, and constraints are defined, the next task is to gather relevant data. This could be achieved via data management systems for precise information or via consultations with stakeholders for rough estimates.
  
  For instance, in the case of the highway management firm setting toll prices for the Chennai-Bangalore Expressway, relevant data could be gathered using FASTag data for vehicles with a valid tag. For vehicles without a tag, data could be gathered through manual traffic counts and toll booth surveys, providing approximations for vehicle flow and toll revenue.

### 3. Formulate the Problem

  A well-defined problem with relevant data enables us to formulate the problem into a concise mathematical model comprising a system of equations that define the cause-effect relationship between the objective function, decision variables, and constraints. Problem formulation is an iterative process of model enrichment, involving model development and validation.
   
  All models are idealized representations of the problem, with necessary approximations and assumptions.

  Below is a typical mathematical model with an objective function $f$, a vector of decision variables $\mathbf{x}$, and a vector of inequality and equality constraints $\mathbf{g},\mathbf{h}$, respecively:

  $$
  \min_{x_1, x_2} \ f(\mathbf{x})
  $$

  Subject to:

  $
  \begin{aligned}
    & \mathbf{g}(\mathbf{x}) \leq 0 \\
    & \mathbf{h}(\mathbf{x}) = 0
  \end{aligned}
  $

  Further, these problems and associated models can be categorized as follows:

  - **Functional Classification**
    - Linear Problem
    - Non-Linear Problem
  - **Temporal Classification**
    - Static Problem
    - Dynamic Problem
  - **Certainty Classification**
    - Deterministic Problem
    - Stochastic Problem

  We shall explore some of these problem formulations in the next lecture.

### 4. Develop and Employ an Optimisation Technique

  Once the problem is formulated, we seek to find values of the decision variables that optimize (maximize or minimize) the objective function while satisfying the constraints. To do this, we can develop and employ either:
  - **Exact methods**, that render the optimal solution (best), or
  - **Approximate methods**, that render a sub-optimal solution (good).
   
  The method deployed depends on the size and complexity of the problem and the computational resources available. We will explore this in future lectures.

  Regardless, it is important to recognize that solutions are best/good only concerning the model being used. Since the model is an idealized representation, there is no guarantee that the best/good solution for the model will be the best/good solution for the real problem. However, if the model is appropriately validated, the resulting solution should be a good approximation for the real-world problem.

### 5. Infer and Implement Results

  The discussion thus far implies that we seek to find only one optimal solution. This, however, is not the case in real-world applications. As discussed, the best/good solution for the modelled problem may not be the best/good solution for the actual problem. Therefore, post-optimality analysis (analysis done after finding an optimal solution) plays a very important role in inferring and implementing the right solution. 
   
  This post-optimality analysis includes what-if analysis to address some questions about what would happen to the optimal solution if different assumptions were made. In part, this post-optimality analysis also involves conducting sensitivity analysis to determine which parameters of the model are most critical in determining the solution, and understanding how the optimal solution would change if the critical parameters changed. 
   
---

This course will focus on defining and formulating problems in Transportation Engineering, developing and employing appropriate optimization techniques, and consequently inferring and implementing the results.
