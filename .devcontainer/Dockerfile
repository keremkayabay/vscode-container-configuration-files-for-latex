# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.138.0/containers/ubuntu/.devcontainer/base.Dockerfile
ARG VARIANT="focal"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${VARIANT}

SHELL ["/bin/bash", "-c"]

# Install additional OS packages.
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends build-essential \
    texlive-full && rm -rf /var/lib/apt/lists/*