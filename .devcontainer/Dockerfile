# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.231.5/containers/alpine/.devcontainer/base.Dockerfile

# [Choice] Alpine version: 3.14, 3.13, 3.12, 3.11
ARG VARIANT="3.15"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-alpine-${VARIANT}

ENV GEM_PATH="/usr/local/rvm/gems/default:/usr/local/rvm/gems/default@global" \
    GEM_HOME="/usr/local/rvm/gems/default" \
    MY_RUBY_HOME="/usr/local/rvm/rubies/default" \
    PATH="/usr/local/rvm/rubies/default/bin:/usr/local/rvm/gems/default@global/bin:/usr/local/rvm/rubies/default/bin:/usr/local/rvm/bin:${PATH}"
COPY library-scripts/ruby-debian.sh /tmp/library-scripts/
RUN apt-get update && bash /tmp/library-scripts/ruby-debian.sh
