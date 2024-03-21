# Use the official Debian slim image
FROM debian:stable-slim

# Install necessary packages
RUN apt-get update && \
    apt-get install -y apt-transport-https gnupg curl unzip  && \
    curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl" && \
    install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl

# Default command to execute when the container starts
CMD ["bash"]

