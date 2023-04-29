ARG VARIANT=20
ARG PLATFORM=linux/amd64
FROM mcr.microsoft.com/devcontainers/javascript-node:0-${VARIANT}

# Install common packages
RUN apt-get update
RUN apt-get install -y git curl wget telnet vim

# Install other packages
# Heroku CLI
RUN curl https://cli-assets.heroku.com/install.sh | sh
