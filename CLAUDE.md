# ComfyUI-ReActor

## Build & Test Commands
- Install dependencies: `python install.py`
- Install on Windows: `install.bat`
- No specific test command available

## Code Style Guidelines

### Imports
- Standard library imports first, then third-party, then local modules
- Use explicit imports for clarity

### Formatting
- Use 4-space indentation
- Follow PEP 8 guidelines for Python code
- Use appropriate docstrings for functions and classes

### Types
- Type hints are helpful but not strictly enforced in existing code
- Class properties should be initialized in `__init__` method

### Naming Conventions
- Classes: PascalCase (e.g., `BuildFaceModel`, `ReActorFaceSwap`)
- Functions/methods: snake_case (e.g., `save_model`, `restore_face`)
- Constants: UPPER_SNAKE_CASE (e.g., `FACE_MODELS_PATH`)
- Variables: snake_case (e.g., `face_model`, `input_image`)

### Error Handling
- Use logger for reporting errors: `logger.error(error_message)`
- Catch specific exceptions rather than broad exception classes

### Node Structure
- Node classes should define `INPUT_TYPES`, `RETURN_TYPES`, `FUNCTION`, and `CATEGORY`
- Main functionality should be in the `execute` method
- Prefer `execute` over custom method names