FROM mcr.microsoft.com/devcontainers/base:1-bookworm

RUN echo 'Acquire::HTTP::Proxy "http://host.docker.internal:3142";' >> /etc/apt/apt.conf.d/01proxy \
 && echo 'Acquire::HTTPS::Proxy "false";' >> /etc/apt/apt.conf.d/01proxy

RUN apt-get update 
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    # Remove imagemagick due to https://security-tracker.debian.org/tracker/CVE-2019-10131
    # && apt-get purge -y imagemagick imagemagick-6-common

ENV LANG=C.UTF-8 \
    LC_ALL=C.UTF-8

USER vscode