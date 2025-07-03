FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Install Java (required by Jenkins)
RUN apt-get update && apt-get install -y openjdk-17-jdk

# Set JAVA_HOME
ENV JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
