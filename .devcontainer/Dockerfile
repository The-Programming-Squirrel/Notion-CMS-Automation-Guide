FROM mcr.microsoft.com/vscode/devcontainers/python:3.10

# Install system dependencies
RUN apt-get update && apt-get install -y \
    pandoc \
    texlive-xetex \
    texlive-fonts-recommended \
    texlive-plain-generic \
    && rm - rf /var/lib/apt/lists/*

# Install Jupyter Book
RUN pip install jupyter-book jupyterlab

# Expose JupyterLab Port
EXPOSE 8888