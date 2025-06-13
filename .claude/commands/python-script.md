# Python script

Create Python scripts that start with the uv script header:

```python
#!/usr/bin/env -S uv run --script

# /// script
# requires-python = ">=3.12"
# ///
```

For scripts with dependencies, include them in the header:

```python
#!/usr/bin/env -S uv run --script

# /// script
# requires-python = ">=3.12"
# dependencies = [
#     "click",
#     "sqlite-utils",
# ]
# ///
```

Run with `uv run <filename.py>`.
