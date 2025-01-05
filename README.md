# How To
Initialize the project
```
uv init --python 3.10 project-name
```

Add venv to the project
```
uv venv --python 3.10
```

Update `pyproject.toml` so that your IDE picks up the python environment of the current project instead of the global environment
```
echo $'\n[tool.pyright]\nvenvPath = "."\nvenv = ".venv"' >> pyproject.toml
```

Add dependency 
```
uv add scipy
```
