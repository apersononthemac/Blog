# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.202.5/containers/ubuntu/.devcontainer/base.Dockerfile

# [Choice] Ubuntu version (use hirsuite or bionic on local arm64/Apple Silicon): hirsute, focal, bionic
ARG VARIANT="hirsute"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${VARIANT}

# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>

RUN sudo curl -OL https://github.com/gohugoio/hugo/releases/download/v0.90.1/hugo_0.90.1_Linux-64bit.tar.gz \
    && sudo tar -xvf hugo_0.90.1_Linux-64bit.tar.gz \
    && sudo mv hugo /usr/bin/hugo \
    && sudo chmod +x /usr/bin/hugo
