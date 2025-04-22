# Use the default Debian-based image
FROM mcr.microsoft.com/devcontainers/base:debian

# Avoid interactive prompts during install
ENV DEBIAN_FRONTEND=noninteractive

# Update and install dependencies
RUN apt-get update && apt-get install -y \
    curl \
    python3 \
    python3-pip \
    git \
    nodejs \
    npm

# Install Vue CLI globally
RUN npm install -g @vue/cli

# Install Flask using pip
RUN pip3 install flask

# Set working directory
WORKDIR /workspace
