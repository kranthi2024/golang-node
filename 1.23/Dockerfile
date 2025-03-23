FROM golang:1.23
RUN apt-get update
RUN apt-get install -y git python3 jq curl
# Install NVM and Node.js
#RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
RUN apt-get update && apt-get install -y zip
# Install Node.js
RUN curl -sL https://deb.nodesource.com/setup_current.x | bash - \
    && apt-get install -y nodejs \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*

# Verify the installations
RUN go version && node -v && npm -v
