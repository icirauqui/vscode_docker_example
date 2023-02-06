# ==================================================================
# module list
# ------------------------------------------------------------------
# Ubuntu           20.04
# ==================================================================

#############################################################################
#                             APT IMAGE + CMAKE                             #
#############################################################################

FROM ubuntu:22.04 as cpu_base_builder

ENV APT_INSTALL="apt-get install -y --no-install-recommends"

RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive $APT_INSTALL \
        build-essential \
        ca-certificates \
        wget \
        git \
        g++ \
        cmake \
        curl zip unzip tar && \
# ==================================================================
# clean up everything
# ------------------------------------------------------------------
    apt-get clean && \
    apt-get -y autoremove && \
    rm -rf /var/lib/apt/lists/*