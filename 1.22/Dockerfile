FROM golang:1.22
RUN apt-get update
RUN apt-get install -y git python3 jq curl

RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash && \
    export NVM_DIR="$HOME/.nvm" && \
    [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" && \
    nvm install 20 && \
    npm install -g gulp && \
    npm install -g yarn

