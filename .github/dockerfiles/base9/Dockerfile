# Base build image of Rocky Linux 9 for slurm build

FROM rockylinux:9

RUN dnf -y update
# not sure if we really need crb, but if we do, we need dnf-plugins-core too:
RUN dnf install -y dnf-plugins-core
RUN dnf -y config-manager --set-enabled crb
RUN dnf -y install rpm-build automake autoconf libtool make pkg-config less vim flex bison cmake which zlib-devel doxygen which wget
