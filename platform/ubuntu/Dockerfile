FROM registry.gitlab.steamos.cloud/steamrt/sniper/sdk  AS base-image

RUN apt update -y
RUN apt install -y build-essential
RUN apt install -y cmake
RUN apt install -y git
RUN apt install -y python3
RUN apt install -y python3-pip
RUN apt install -y zip
RUN apt install -y curl
RUN apt install -y unzip
RUN apt install -y pkg-config
RUN apt install -y autoconf
RUN apt install -y libtool
RUN apt install -y flex
RUN apt install -y bison
RUN pip3 install scons

FROM registry.gitlab.steamos.cloud/steamrt/sniper/sdk
COPY --from=base-image / /
