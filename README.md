![Build Status](https://github.com/petrdokladal/fast_math_project/actions/workflows/build_wheels.yml/badge.svg)

## Installation

This project uses [uv](https://docs.astral.sh/uv/) for extremely fast dependency management and environment isolation.

### 1. Install uv (if needed)
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Initialize uv's environment variables

```bash
source $HOME/.local/bin/env

uv init
```

Create a python environment (using a pyhon version of your choice)

```bash
uv venv --python 3.14
```

Activate the environment
```bash
source .venv/bin/activate
```
Install locally using the wheel from github. 
```bash
uv pip install -e .
```

Test the code

```bash
python3 -c "import fast_math; print(fast_math.multiply(5, 5))"
```

You can also run the code without activating the environment
```bash
uv run python3 -c "import fast_math; print(fast_math.multiply(5, 5))"
```

