FROM ubuntu:20.04

# Install dependencies
RUN apt-get update && apt-get install -y \
    curl \
    build-essential \
    ca-certificates \
    libssl-dev \
    pkg-config \
    nodejs \
    npm \
    git \
    rustc \
    cargo

# Install DFX (Dfinity SDK)
RUN curl -o- https://internetcomputer.org/install.sh | sh

# Add DFX to the path
ENV PATH="/root/bin/:${PATH}"

# Set working directory
WORKDIR /workspace
