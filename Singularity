Bootstrap: docker
From: ubuntu:bionic


%post
    mkdir -p /tmp/cellranger-build \
    && cd /tmp/cellranger-build \
    && apt-get update \
    && apt-get install -y wget \
    && wget -O cellranger-4.0.0.tar.gz "https://cf.10xgenomics.com/releases/cell-exp/cellranger-4.0.0.tar.gz?Expires=1605584822&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9jZi4xMHhnZW5vbWljcy5jb20vcmVsZWFzZXMvY2VsbC1leHAvY2VsbHJhbmdlci00LjAuMC50YXIuZ3oiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE2MDU1ODQ4MjJ9fX1dfQ__&Signature=dLeOXCuNyUQAgcL0YbHMzlAfTtwPjOwaHOtJIxNqIpRqn3osRQLkZqrYjtIbtl8mTn0tVRgm45uYnhivWf9RsvFm3URTjEBDH5PeSbLlanV7CCPVYJwdxopamg4Rq7GUx~GVN2aEUOVCFpARU2PJA6jf4S42atgS3XI3LkkK7Z2fDhL88fcpOd9DyoBpE0NFxD2Mf0NrffRzL4B009dPzszUhTU9qv9tS-JfI~so9wxhQ10gDRD9hH3uxRz~W4HafRgzHdJjjYAZyGzL2Zwgi6z-QR5gDR1yeHsMFG1m9HAII4D06nNSfYReOrf1b9OzWCX2Dlia2nVq-TLRCxzSeQ__&Key-Pair-Id=APKAI7S6A5RYOXBWRPDA" \
    && mkdir /apps \
    && mv cellranger-4.0.0.tar.gz /apps/ \
    && cd /apps \
    && tar -xzvf cellranger-4.0.0.tar.gz \
    && rm -f cellranger-4.0.0.tar.gz \
    && rm -rf /tmp/cellranger-build

%environment
    export PATH=/apps/cellranger-4.0.0:$PATH

%labels
    Alessandro Raveane
    Version v0.0.1

