
## Heat-generation case (v1.1)

The equation is now $d^2T/dx^2 = -S$, where $S = \dot q/k$.
L = 1 m, T_L = 100 C, T_R = 30 C, S = 80 K/m², 101 nodes.
Expected midpoint: 75.0 C. With S = 0 (v1.0), it is 65.0 C.
Run `python src/verify_case.py` and `python src/run_case.py`.
