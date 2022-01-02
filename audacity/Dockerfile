FROM  ubuntu:20.04
MAINTAINER David Marteau <david.marteau@3liz.com>
LABEL Description="Audacity software" Version="22.01.0"

RUN apt-get update && apt-get upgrade -y && apt-get install -y --no-install-recommends \
        software-properties-common \
        pulseaudio \
    && add-apt-repository ppa:ubuntuhandbook1/audacity \
    && apt-get update \
    && apt-get install -yq --no-install-recommends audacity \
    && rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["audacity"]

