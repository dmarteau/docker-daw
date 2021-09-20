FROM  ubuntu:20.04
MAINTAINER David Marteau <david.marteau@3liz.com>
LABEL Description="LMMS software" Version="21.09.0"

RUN apt-get update && apt-get upgrade -y && apt-get install -y --no-install-recommends \
    && apt-get install -yq --no-install-recommends lmms pulseaudio \
    && rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["lmms"]
