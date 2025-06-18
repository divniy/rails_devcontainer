# Rails devcontainer image 
Replacement for ```ghcr.io/rails/devcontainer/images/ruby:$RUBY_VERSION```

Change content ```.devcontainer/Dockerfile``` with

```
# Make sure RUBY_VERSION matches the Ruby version in .ruby-version
ARG RUBY_VERSION=3.4.4
FROM ghcr.io/divniy/devcontainers/images/ruby:$RUBY_VERSION
```