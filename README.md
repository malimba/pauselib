# pauselib

A tiny Python utility library for **pausing with style** — timed waits, animated messages, and input timeouts when bare `time.sleep()` isn't enough.

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white)

## Why?

Ever wrapped everything in `try/except` just to rerun on failure? Or wanted a countdown with a message before retrying? **pauselib** gives you readable pause helpers without boilerplate.

## Features

- `pause(seconds)` — simple sleep wrapper
- `with_msg(seconds, message)` — wait with a printed message
- `for_input(seconds)` — timed input prompts
- Custom exception types in `exceptions.py`
- Test harness under `tests/`

## Quick start

```python
from pause import pause

pause.pause(3)
pause.with_msg(5, "Retrying in…")
pause.for_input(10)
```

Or explore interactively:

```bash
python test.py
```

## Project layout

```
pause.py         # Main API
core/            # Implementation details
exceptions.py    # Custom error types
tests/           # Test cases
```

---

[malimba](https://github.com/malimba)
