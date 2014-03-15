#
# Core Dockerfile for UberConverter
#
# pandoc
# 
FROM ubuntu:12.04
MAINTAINER UberConverter <admin@uberconverter.com>

# Hook up repositories:
RUN echo "deb http://archive.ubuntu.com/ubuntu $(lsb_release -sc) main universe" > /etc/apt/sources.list

# install haskell
RUN apt-get update -y && apt-get install -y haskell-platform
# install pandoc
RUN cabal update && cabal install pandoc pandoc-citeproc
# e.g. to install a specific version:
#RUN cabal update && cabal install pandoc-1.12.3.2

# install latex packages
RUN apt-get update -y && apt-get install -y texlive-latex-base texlive-xetex latex-xcolor texlive-math-extra texlive-latex-extra texlive-fonts-extra biblatex curl wget git fontconfig make


# Set up invocation hooks:
RUN mkdir -p /source
WORKDIR /source

ENTRYPOINT ["/.cabal/bin/pandoc"]
CMD ["--help"]

