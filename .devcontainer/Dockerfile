FROM mcr.microsoft.com/vscode/devcontainers/javascript-node:0-18

# Install system dependencies for React Native
RUN apt-get update && apt-get install -yq libglu1-mesa-dev libgles2-mesa-dev \
    libegl1-mesa-dev libx11-dev

# Set up environment variables
ENV ADB_IP="host.docker.internal"

# Install Expo CLI
RUN npm install -g expo-cli react-native-cli

# Set the working directory
WORKDIR /workspace
