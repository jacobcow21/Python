# https://github.com/devcontainers/images/tree/main/src/python
# Mirrors the image used by devcontainer.json. Dependencies live in
# pyproject.toml/uv.lock (there is no requirements.txt), so contributors
# install them with `uv sync` inside the container.
ARG VARIANT=latest
FROM mcr.microsoft.com/devcontainers/python:${VARIANT}
RUN pipx install pre-commit \
  && pipx install ruff \
  && pipx install uv
