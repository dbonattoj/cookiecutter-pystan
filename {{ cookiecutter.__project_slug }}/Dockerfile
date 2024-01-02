# Base image
FROM python:3.10

# Install required packages
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    g++ \
    gcc \
    build-essential \
    && rm -rf /var/lib/apt/lists/*


# Set working directory
WORKDIR ${workspaceFolder}

