# mdgpt (starter)

This is a minimal, deterministic MD project generator:
- Input: a single `spec.yaml`
- Output: a reproducible project folder (`mdp/`, `scripts/`, `slurm/`, `manifest.json`, `validate.md`)

## Quickstart

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -e .

mdgpt init examples/protein_water/spec.yaml -o run1
```

Open `run1/validate.md` and `run1/README.md`.

## What this starter does NOT do (yet)
- Build the system (pdb2gmx/solvate/genion/index) end-to-end
- Run GROMACS automatically
- Handle ligands/membranes/umbrella sampling

Those come next once the scaffold is solid and trusted.
