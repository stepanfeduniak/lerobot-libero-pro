# LeRobot × LIBERO-PRO Integration

Minimal glue code to use **LIBERO-PRO** through **LeRobot**.

## Upstream projects

- LIBERO-PRO: https://github.com/Zxy-MLlab/LIBERO-PRO  
- LeRobot LIBERO: https://github.com/huggingface/lerobot-libero

## Install

### Option A: install this integration directly instead of libero.

```bash
pip install "libero @ git+https://github.com/stepanfeduniak/lerobot-libero-pro.git"
```

### Option B: add as a LeRobot extra

Add this to LeRobot’s `pyproject.toml` under the extras section:

```toml
libero-pro = ["lerobot[transformers-dep]","libero @ git+https://github.com/stepanfeduniak/lerobot-libero-pro.git"]
```

Then install from your local LeRobot:

```bash
pip install -e ".[libero-pro]"
```
