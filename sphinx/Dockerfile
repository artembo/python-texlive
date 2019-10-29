FROM python:3.7

LABEL maintainer="Artem Morozov <artembo@me.com>"

RUN apt-get update && apt-get -y install --no-install-recommends --no-install-suggests \
 texlive \
 texlive-lang-cyrillic \
 texlive-latex-extra \
 texlive-fonts-extra \
 texlive-extra-utils \
 imagemagick \
 inkscape \
 xzdec \
 cmake \
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/*

RUN pip install sphinx==1.8.5 sphinx-intl sphinx_rtd_theme awscli

RUN mkdir /doc
WORKDIR /doc