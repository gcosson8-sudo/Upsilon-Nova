FROM debian:bullseye-slim

RUN apt-get update && \
  apt-get install -y --no-install-recommends \
  build-essential git imagemagick libx11-dev libxext-dev libfreetype6-dev libpng-dev libjpeg-dev pkg-config gcc-arm-none-eabi binutils-arm-none-eabi ca-certificates python3 && \
  apt-get clean

COPY ./build /

ENTRYPOINT ["/build"]
