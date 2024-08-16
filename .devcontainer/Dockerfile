FROM redhat/ubi9
WORKDIR /

RUN dnf update -y

# Install build tools for DSS
RUN dnf intall -y \
        apr-devel \
        apr-util \
        apr-util-devel && \
        dnf clean all

# Add user
RUN useradd -m vscode
USER vscode