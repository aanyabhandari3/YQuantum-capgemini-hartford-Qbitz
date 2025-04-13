# YQuantum-capgemini-hartford-Qbitz

# QEdge Portfolio (VQE)
## Inspiration
Insurance companies like The Hartford manage portfolios of insured properties where correlated risks (e.g., from natural disasters) can lead to major losses. We were inspired to explore how **quantum computing**, particularly **Variational Quantum Eigensolver (VQE)**, can help optimize such portfolios for lower total risk while maintaining high return.

## What it does
QEdge Portfolios selects the optimal subset of properties (out of many) by:
- Minimizing total correlation risk (from a correlation matrix)
- Maximizing expected return
- Enforcing a strict budget (select exactly B properties)

The system compares three solutions:
- Random selection
- Classical solver (CVXPY)
- Quantum-enhanced selection using VQE

## How we built it
- Formulated the problem as a **QUBO** (Quadratic Unconstrained Binary Optimization)
- Converted to **Ising Hamiltonian** for quantum evaluation
- Implemented VQE with **PennyLane** and a parametrized quantum circuit
- Benchmarked against classical solutions using **CVXPY**
- Visualized energy convergence, portfolio choices, and comparative performance

## Challenges we ran into
- CVXPY solver compatibility required tuning and fallbacks
- Mapping QUBO to Ising with penalties required care to enforce the budget
- Quantum circuit design needed to balance expressive power and convergence stability
- Interpreting quantum measurement results into actionable portfolio decisions

## Accomplishments that we're proud of
- Developed a full quantum-classical pipeline to solve a real business problem
- Achieved measurable improvement over both random and classical baselines
- Demonstrated the feasibility of running VQE on practical insurance data
- Created a reusable framework scalable to IBM Q or Braket

## What we learned
- VQE is a powerful hybrid method even on today’s NISQ devices
- Penalty methods can enforce hard constraints in quantum optimization
- Classical post-processing is key to interpreting quantum results
- Domain-specific quantum optimization is already valuable

## What's next for QEdge Portfolios
- Scale the model to 50+ properties
- Add real-world insurance data from The Hartford
- Introduce ESG and exposure constraints
- Deploy to real quantum backends (IBM Q, Rigetti, Braket)
- Create a front-end interface for actuaries to interact with quantum optimization results

## Authors
- Aanya Bhandari
- Roman Tudor
- Felix Caron
- Victor Rochon
- Jacopo Dardini

