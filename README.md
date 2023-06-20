A test repo to reproduce a crash in the ruff vscode extension

Tested on python 3.10.4 and 3.11.3 using ruff 0.0.272

To reproduce:

1. install [poetry](https://python-poetry.org/)
2. run `poetry config virtualenvs.in-project true`
3. navigate to libs/a_lib or services/b_service and run `poetry install`
4. open the vscode workspace, have the ruff vscode extension installed, and open a.py or b_service.py
5. ruff extension fails with `Server: Start failed: Error: Unsupported server configuration`