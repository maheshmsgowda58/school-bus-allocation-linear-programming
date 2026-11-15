
# School Bus Allocation Optimization Using Linear Programming

## 📌 Project Description

The School Bus Allocation Optimization project is a Python-based Operations Research project that uses Linear Programming (LP) to determine the most cost-effective combination of large and small buses for transporting 400 students.

The transportation company has 10 large buses with 50 seats each and 8 small buses with 40 seats each. However, only 9 drivers are available.

The objective is to minimize the total transportation rental cost while satisfying the student seating requirements, bus availability constraints, and driver limitations.

The optimization problem is implemented using Python and the PuLP library. The project also visualizes the feasible region and optimal solution using Matplotlib.

## 🎯 Project Objectives

- Understand Linear Programming concepts.
- Formulate a real-world transportation optimization problem.
- Define decision variables and objective functions.
- Establish resource and capacity constraints.
- Minimize total transportation costs.
- Solve integer optimization problems using PuLP.
- Visualize feasible solutions and optimal allocation.

## 🛠️ Technologies Used

- Python
- PuLP
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📂 Project Structure

```text
School-Bus-Allocation-Optimization/
│
├── BusProblem.ipynb
└── README.md
```

## 📋 Problem Statement

A school is preparing a trip for 400 students.

The transportation company has:

- 10 large buses with 50 seats each.
- 8 small buses with 40 seats each.
- Only 9 drivers available.
- Large bus rental cost: 800.
- Small bus rental cost: 600.

The objective is to calculate how many large and small buses should be used to transport all 400 students at the minimum possible cost.

## 🧮 Mathematical Formulation

### Decision Variables

Let:

- x = Number of large buses.
- y = Number of small buses.

### Objective Function

Minimize the total transportation cost:

```text
Minimize Z = 800x + 600y
```

### Constraints

**1. Seating Capacity Constraint**

All 400 students must have seats.

```text
50x + 40y >= 400
```

**2. Driver Availability Constraint**

A maximum of 9 drivers are available.

```text
x + y <= 9
```

**3. Large Bus Availability**

```text
0 <= x <= 10
```

**4. Small Bus Availability**

```text
0 <= y <= 8
```

**5. Integer Constraint**

```text
x, y >= 0
```

Both decision variables must be non-negative integers because buses cannot be fractional.

## ⚙️ Project Workflow

### 1. Import Libraries

Import the required Python libraries:

- PuLP for Linear Programming.
- NumPy for numerical operations.
- Pandas for data handling.
- Matplotlib and Seaborn for visualization.

### 2. Define the Optimization Problem

Create a Linear Programming minimization problem using PuLP.

### 3. Define Decision Variables

Create two integer decision variables:

- Large buses (x).
- Small buses (y).

Define their minimum and maximum limits based on bus availability.

### 4. Define the Objective Function

Minimize the total rental cost:

```python
prob += 800 * x + 600 * y
```

### 5. Add Constraints

Add the following constraints:

- Student seating capacity.
- Maximum number of available drivers.
- Large bus availability.
- Small bus availability.

### 6. Solve the Optimization Problem

Use the PuLP solver to find the optimal combination of buses.

### 7. Extract the Optimal Solution

Retrieve:

- Number of large buses.
- Number of small buses.
- Minimum total transportation cost.

### 8. Visualize the Results

Use Matplotlib to visualize:

- Seating capacity constraint.
- Driver availability constraint.
- Feasible region.
- Optimal solution point.

## 🔄 Optimization Workflow

```text
       Problem Definition
               |
               v
       Define Variables
               |
               v
      Objective Function
               |
               v
       Define Constraints
               |
               v
      Linear Programming
               |
               v
        PuLP Solver
               |
               v
       Optimal Solution
               |
               v
       Cost Calculation
               |
               v
       Result Visualization
```

## 📊 Optimal Solution

The optimal solution is:

| Parameter | Result |
|---|---:|
| Students | 400 |
| Large buses used | 4 |
| Small buses used | 5 |
| Total buses used | 9 |
| Total seats available | 400 |
| Drivers required | 9 |
| Large bus cost | 3,200 |
| Small bus cost | 3,000 |
| Minimum total cost | 6,200 |

### Cost Calculation

```text
Large Bus Cost = 4 × 800 = 3,200

Small Bus Cost = 5 × 600 = 3,000

Total Cost = 3,200 + 3,000

Minimum Total Cost = 6,200
```

The solution satisfies all the seating capacity, driver availability, and bus availability constraints.

## 📈 Visualization

The project generates a graphical representation of the optimization problem.

The visualization includes:

- Feasible region representing valid bus combinations.
- Seating capacity constraint line.
- Driver availability constraint line.
- Optimal solution point.

This visualization helps understand how Linear Programming identifies the minimum-cost solution.

## 📦 Installation

Install Python and the required libraries:

```bash
pip install pulp pandas numpy matplotlib seaborn
```

## ▶️ How to Run

Clone the repository:

```bash
git clone <your-repository-url>
```

Navigate to the project folder:

```bash
cd School-Bus-Allocation-Optimization
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook:

```text
BusProblem.ipynb
```

Run all cells to execute the optimization problem and visualize the results.

## 💡 Key Learnings

- Fundamentals of Operations Research.
- Linear Programming concepts.
- Objective function formulation.
- Decision variables.
- Equality and inequality constraints.
- Integer Programming.
- Cost minimization techniques.
- Resource allocation optimization.
- Solving optimization problems using PuLP.
- Feasible region visualization using Matplotlib.

## 🚀 Future Improvements

- Solve more complex transportation optimization problems.
- Include multiple vehicle types and transportation routes.
- Add fuel and maintenance costs.
- Build an interactive optimization dashboard.
- Compare different optimization algorithms.
- Integrate real-time transportation requirements.

## 📝 Conclusion

The School Bus Allocation Optimization project demonstrates how Linear Programming can solve real-world resource allocation and cost minimization problems.

By defining decision variables, objective functions, and constraints, the project identifies the optimal combination of large and small buses required to transport 400 students at the minimum possible rental cost.

The project provides practical experience in mathematical optimization, integer programming, Operations Research, and Python-based problem-solving.

---

**Project Name:** School Bus Allocation Optimization Using Linear Programming

**Domain:** Operations Research / Optimization

**Programming Language:** Python

**Optimization Library:** PuLP

**Problem Type:** Integer Linear Programming

**Objective:** Cost Minimization
