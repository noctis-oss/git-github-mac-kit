
## How to run

    python3 -m venv .venv
    source .venv/bin/activate
    python -m pip install -r requirements.txt
    python src/verify_case.py
    python src/run_case.py

| Folder   | Holds                              |
|----------|------------------------------------|
| theory/  | the derivation                     |
| src/     | solver, exact solution, checks     |
| results/ | the temperature table (generated)  |
| figures/ | the comparison figure (generated)  |
