# Use the default Debian-based image
FROM mcr.microsoft.com/devcontainers/base:debian

# Avoid interactive prompts during install
ENV DEBIAN_FRONTEND=noninteractive

Install curl and dependencies
RUN apt-get update && \
    apt-get install -y curl python3 python3-pip

# Install Node.js and Vue CLI
RUN curl -fsSL https://deb.nodesource.com/setup_20.x | bash - && \
    apt-get install -y nodejs && \
    npm install -g @vue/cli

# Install Flask with --break-system-packages
RUN pip3 install flask --break-system-packages

# Set working directory
WORKDIR /workspace
