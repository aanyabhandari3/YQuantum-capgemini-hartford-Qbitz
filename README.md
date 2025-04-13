# YQuantum-capgemini-hartford-Qbitz

# Quantum Insurance Portfolio Optimization (Alpha-VQE)

This project uses **Alpha-VQE**, a hybrid quantum-classical variational algorithm, to optimize an insurance portfolio by selecting a subset of properties that:

- Maximize return
- Minimize correlation-based risk
- Respect a strict budget constraint

The approach is benchmarked against both **random selection** and a **classical solver**, demonstrating quantum-enhanced performance in complex decision spaces relevant to real-world insurance operations.

---

## Problem Context

Insurance companies like **The Hartford** must construct property portfolios that:

- Avoid **correlated risk exposure** (e.g., properties in the same flood zone)
- Maximize **expected returns** from premiums
- Select exactly **B properties** within capital or regulatory limits

Mathematically, this is a **Quadratic Unconstrained Binary Optimization (QUBO)** problem, which is NP-hard and becomes intractable for large portfolios using classical solvers.

---

## Quantum Solution (Alpha-VQE)

We model the QUBO as an **Ising Hamiltonian**:

---

## Authors

- Aanya Bhandari
- Roman Tudor
- Felix Caron
- Victor Rochon
- X

