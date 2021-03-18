ARG VARIANT="14-buster"
FROM mcr.microsoft.com/vscode/devcontainers/javascript-node:0-${VARIANT}

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends jupyter

RUN su node -c "npm install -g ijavascript"
RUN su node -c "ijsinstall"