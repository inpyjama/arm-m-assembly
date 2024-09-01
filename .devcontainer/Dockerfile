#
# Copyright © 2024 inpyjama.com. All Rights Reserved.
# Author: Piyush Itankar <piyush@inpyjama.com>
#

FROM mcr.microsoft.com/vscode/devcontainers/base:ubuntu

ENV DEBIAN_FRONTEND=noninteractive

RUN sudo apt-get update
RUN sudo apt-get install --no-install-recommends -y \
  sudo \
  binutils-common \
  make \
  git-core \
  wget \
  tree \
  build-essential \
  python3 \
  python3-dev \
  python3-pip \
  binutils \
  make \
  qemu-system-arm \
  gcc-arm-none-eabi \
  gdb-multiarch

RUN pip install pygments
RUN wget -P ~ https://git.io/.gdbinit

# terminal colors with xterm
ENV TERM xterm