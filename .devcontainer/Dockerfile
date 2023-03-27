FROM mcr.microsoft.com/devcontainers/python:0-3.11

# Essentials
RUN apt-get update

RUN apt-get install -y \
    build-essential \
    curl \
    cmake

RUN apt-get update

# Switch to vscode user
USER vscode 
# Get Rust
RUN curl https://sh.rustup.rs -sSf | bash -s -- -y
ENV PATH="/home/vscode/.cargo/bin:${PATH}"

RUN pip install --upgrade pip

